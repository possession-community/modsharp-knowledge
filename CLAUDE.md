# modsharp-knowledge — Claude Code runbook

This repository stores the API catalog for ModSharp
(CS2 / Source 2 C# modding framework). Catalog generation and
updates are executed by Claude Code following this runbook.

## Prerequisites
- .NET 10 SDK installed
- The catalog generator tool is available locally.
  Source: <https://github.com/fltuna/modsharp-api-catalog-generator>

  Default expected path: `~/tools/ModSharpApiCatalog`.
  Override with the environment variable `MODSHARP_CATALOG_TOOL`.

  If the tool is missing, ask the user to clone it first:
  ```bash
  git clone https://github.com/fltuna/modsharp-api-catalog-generator.git \
      ~/tools/ModSharpApiCatalog
  ```
  The directory name can be anything; `MODSHARP_CATALOG_TOOL`
  (or the path passed to `--project`) just has to point at it.
  If still not available after cloning, stop and tell the user.

## Procedure when the user asks you to update the catalog

### Step 1: check for upstream changes
```bash
cd external/modsharp
git fetch origin
LOCAL=$(git rev-parse HEAD)
REMOTE=$(git rev-parse origin/master)
```
- If `LOCAL == REMOTE`, there are no updates. Report that and stop.
- Otherwise, show `git log --oneline $LOCAL..$REMOTE | head -20` so the user sees what changed.

### Step 2: update the submodule
From the repo root:
```bash
cd <repo root>
git submodule update --remote external/modsharp
```

### Step 3: build ModSharp (needed so Source-Generator output is available)
```bash
cd external/modsharp
dotnet restore
dotnet build --no-restore --configuration Release
```
- If the build fails, report the error and wait for direction.
- Without a successful build, Source-Generator-emitted types will be missing from the catalog.

### Step 4: generate the catalog
ModSharp currently has no `.sln` — just `.csproj` files and a
`Directory.Build.props`. The tool uses `--scan` to discover them.
```bash
cd <repo root>
TOOL_PATH="${MODSHARP_CATALOG_TOOL:-$HOME/tools/ModSharpApiCatalog}"
dotnet run --project "$TOOL_PATH" --configuration Release -- \
    --scan external/modsharp \
    --output catalog \
    --source-root external/modsharp
```
If upstream ever adds a `.sln`, `--solution <path>` also works.

### Step 5: review the diff
```bash
git status
git diff --stat catalog/
```
Summarize the change for the user.

### Step 6: commit (after the user approves)
```bash
NEW_COMMIT=$(cd external/modsharp && git rev-parse --short HEAD)
git add -A
git commit -m "Update catalog to ModSharp $NEW_COMMIT"
```
Leave `git push` to the user's judgement.

## Fresh-machine bootstrap
If the repo was cloned without `--recurse-submodules`:
```bash
git submodule update --init --recursive
```

## Troubleshooting

### MSBuildWorkspace fails to load
Verify that the tool calls `Microsoft.Build.Locator.RegisterDefaults()`
before touching any MSBuild or Workspaces type. If the tool itself
needs a fix, report to the user.

### Source-Generator types are missing from the catalog
- Confirm Step 3 succeeded.
- Check that `catalog/indexes/generated-types.md` is not empty.
- If it is empty, the tool implementation needs a look.

### The catalog tool cannot be found
- Check `MODSHARP_CATALOG_TOOL`.
- Check the default path `~/tools/ModSharpApiCatalog`.
- If neither works, ask the user where the tool lives.

## Invariants
- Source Generator output (`*.g.cs` etc.) is always included in the catalog — never excluded.
- `catalog/.meta/generated-at` is volatile and gitignored.
- A failed ModSharp build means an incomplete catalog.
- `patterns/` and `gotchas.md` are hand-maintained. Do not auto-generate or rewrite them without an explicit instruction from the user.

## Language policy
All hand-written content in this repo is written in **English**:
`CLAUDE.md`, `README.md`, files under `docs/` and `patterns/`,
`gotchas.md`, and commit messages. Keep any new additions in English
even if the conversation driving the change is happening in another
language.

## What you may edit / must not edit

### Editable
- `catalog/` — only via the generator tool; never hand-edit
- `patterns/` — only when the user asks explicitly
- `gotchas.md` — only when the user asks explicitly
- `README.md`, `docs/usage.md`, this `CLAUDE.md`

### Off-limits
- Anything under `external/modsharp/` (submodule contents)
- `.gitmodules`
