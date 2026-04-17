# init.md — Setup runbook for plugin consumers

**Audience:** you are Claude Code running inside a **plugin project**
that has added `modsharp-knowledge` as a submodule at `refs/modsharp-knowledge`.
The user pointed you at this file. Your job: wire the catalog into the
plugin's own `CLAUDE.md`, interactively.

If you are running inside the `modsharp-knowledge` repo itself, this is
the wrong file — stop and tell the user.

## Step 1: verify environment
1. Confirm that `refs/modsharp-knowledge/catalog/_index.md` exists
   relative to the plugin repo root. If not, tell the user the submodule
   isn't checked out and stop.
2. Locate the plugin's `CLAUDE.md`:
   - If `CLAUDE.md` exists at the plugin root, use it.
   - If not, **ask the user before creating one** — creating `CLAUDE.md`
     affects every future Claude Code session in the repo.

## Step 2: ask the user which preset to apply
Use the `AskUserQuestion` tool (or an equivalent interactive prompt).
Present these options and default to **Full** if the user doesn't care:

| Option | What it does |
|---|---|
| **Full** (recommended) | Always-on `@`-refs + workflow checklist + browse list + notes |
| **Minimal** | Only the always-on `@`-refs (`_index.md`, `gotchas.md`) |
| **Custom** | Walk through each block and ask per item |
| **Cancel** | Do nothing |

## Step 3: check for an existing integration
Search the plugin `CLAUDE.md` for the marker:

```
<!-- BEGIN modsharp-knowledge integration -->
```

- If present: ask the user whether to **replace** the existing block or **skip**.
- If absent: continue.

## Step 4: compose the snippet
Assemble the block the user chose. Always wrap it with the BEGIN / END
markers so a later re-run of this runbook can locate and replace it.

### Full preset

```markdown
<!-- BEGIN modsharp-knowledge integration -->
## ModSharp reference material

Auto-loaded at session start (keep each `@` on its own line, with
no trailing prose on the same line — Claude Code parses the rest of
the line as part of the path):

@refs/modsharp-knowledge/catalog/_index.md
@refs/modsharp-knowledge/gotchas.md

Browse on demand (plain paths — do NOT prefix with `@`):
- `refs/modsharp-knowledge/catalog/projects/Sharp.Shared/_index.md`
- `refs/modsharp-knowledge/catalog/projects/Sharp.Shared/namespaces/`
- `refs/modsharp-knowledge/catalog/indexes/`
- `refs/modsharp-knowledge/patterns/`

## Workflow when touching ModSharp APIs
1. Start from `refs/modsharp-knowledge/catalog/_index.md` to find the right project.
2. Read `refs/modsharp-knowledge/catalog/projects/Sharp.Shared/_index.md` to locate the namespace.
3. Read the relevant `namespaces/<Namespace>.md` file for type signatures.
4. Check `refs/modsharp-knowledge/patterns/` for a verified precedent.
5. Scan `refs/modsharp-knowledge/gotchas.md` before committing tricky code.

## Notes
- Never auto-load `catalog/projects/*/namespaces/*.md` with `@` — some files exceed 60k lines and will blow the context window.
- Pull catalog updates with `git submodule update --remote refs/modsharp-knowledge`.
<!-- END modsharp-knowledge integration -->
```

### Minimal preset

```markdown
<!-- BEGIN modsharp-knowledge integration -->
## ModSharp reference material

Auto-loaded at session start (one `@` per line, nothing else on the line):

@refs/modsharp-knowledge/catalog/_index.md
@refs/modsharp-knowledge/gotchas.md

Never auto-load per-namespace files — some exceed 60k lines.
<!-- END modsharp-knowledge integration -->
```

### Custom preset
Offer these blocks individually and assemble only the ones the user chooses:

- **Always-on refs** — the two `@`-lines for `_index.md` and `gotchas.md`
- **Browse-on-demand list** — paths to directories Claude should read on demand
- **Workflow checklist** — the 5-step workflow
- **Notes** — the "never auto-load large files" reminder and update command

Whichever blocks the user picks, wrap the final output with the same
BEGIN / END markers.

## Step 5: write the change
- If `CLAUDE.md` exists:
  - If the marker already existed and the user chose **replace**, substitute
    the block between the markers (inclusive).
  - Otherwise, append a blank line and the new block at the end of the file.
- If `CLAUDE.md` does not exist and the user approved creating one:
  - Create the file containing only the chosen block.

## Step 6: summarize and stop
Report back:
- Which file you touched.
- Which preset you applied.
- The lines you added or replaced.

**Do not commit** — leave that to the user so they can review the diff
first.

## Language policy
The snippets above are in English. Even if the user is speaking another
language with you, keep the inserted block in English for consistency
with the rest of the catalog.
