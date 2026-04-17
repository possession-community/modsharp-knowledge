# Usage

## Update workflow
Catalog updates happen inside a Claude Code session. No shell scripts
or CI automation are provided on purpose.

1. Open a Claude Code session in this repository.
2. Tell Claude "update the catalog" (or something equivalent).
3. Claude Code follows `CLAUDE.md` and runs the commands itself.
4. Review the diff and commit.

## Consuming the catalog from a plugin project

### 1. Add as a submodule
```bash
cd my-plugin
git submodule add <this-repo-url> refs/modsharp-catalog
git commit -m "Add ModSharp catalog reference"
```

### 2. Reference it from the plugin's `CLAUDE.md`
The catalog is large. Some files are small and worth loading into
context at session start (`@path` references); others are big and
should only be read on demand.

Recommended snippet to paste into the plugin's `CLAUDE.md`:

```markdown
## ModSharp reference material

Always-on context (loaded at session start via `@`):
- @refs/modsharp-catalog/catalog/_index.md   — top-level index
- @refs/modsharp-catalog/gotchas.md          — small, always worth keeping hot

Browse on demand (do NOT auto-load with `@`):
- refs/modsharp-catalog/catalog/projects/Sharp.Shared/_index.md
- refs/modsharp-catalog/catalog/projects/Sharp.Shared/namespaces/
- refs/modsharp-catalog/catalog/indexes/
- refs/modsharp-catalog/patterns/

## Workflow when touching ModSharp APIs
1. Start from @refs/modsharp-catalog/catalog/_index.md to find the right project.
2. Read `refs/modsharp-catalog/catalog/projects/Sharp.Shared/_index.md` to locate the namespace.
3. Read the relevant `namespaces/<Namespace>.md` file for type signatures.
4. Check `refs/modsharp-catalog/patterns/` for a verified precedent before writing new code.
5. Scan `@refs/modsharp-catalog/gotchas.md` before committing anything non-trivial.
```

### Which files to reference — cheat sheet

| File / directory | Typical size | `@`-load? | Notes |
|---|---|---|---|
| `catalog/_index.md` | small | **Yes** | Top-level index, always useful |
| `gotchas.md` | small | **Yes** | Worth keeping hot |
| `catalog/projects/Sharp.Shared/_index.md` | medium | No | Link and let Claude read on demand |
| `catalog/projects/Sharp.Shared/namespaces/*.md` | **large** (`_global.md` exceeds 60k lines) | **Never** | Auto-loading will blow context |
| `catalog/indexes/entry-points.md` | medium | Optional | Useful to pin during scaffolding |
| `catalog/indexes/generated-types.md` | medium | Optional | Useful when working with protobuf / generated code |
| `patterns/` | small per file | Directory ref | Claude reads individual patterns as needed |

A plugin consumer only needs the submodule. The generator tool at
`~/tools/ModSharpApiCatalog` is required for **updating** the catalog,
not for **consuming** it.

### 3. Pull catalog updates into the plugin
When the plugin wants a fresher catalog:
```bash
git submodule update --remote refs/modsharp-catalog
git commit -am "Update catalog reference"
```

## Cloning on a new machine
```bash
git clone --recurse-submodules <plugin-repo-url>
```
Don't forget `--recurse-submodules`. You can make it the default with
`git config --global submodule.recurse true`.

## Note: testing submodule wiring against a local path
Modern git refuses `file://` submodule clones by default. When wiring
this catalog into a throwaway test project on the same filesystem,
allow it for that single command:
```bash
git -c protocol.file.allow=always submodule add /path/to/modsharp-catalog refs/modsharp-catalog
```
HTTPS-hosted submodules don't need this.
