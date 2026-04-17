# ModSharp Knowledge

API catalog and curated development knowledge for ModSharp
(CS2 / Source 2 C# modding framework).

## Purpose
- Let AI assistants (Claude Code and similar) see the full public API of ModSharp so their suggestions stay grounded in what actually exists
- Provide a complete view that includes Source-Generator-emitted types (protobuf stubs, entity metadata, etc.)
- Collect verified usage patterns
- Record gotchas to stop the same mistakes from recurring

## Layout
- `external/modsharp/` — ModSharp source as a pinned git submodule
- `catalog/` — auto-generated API catalog (includes Source Generator output)
- `patterns/` — verified usage patterns, maintained by hand
- `gotchas.md` — gotchas / pitfalls, maintained by hand
- `CLAUDE.md` — the runbook Claude Code follows when updating the catalog
- `docs/usage.md` — how to consume this catalog from a plugin project

## Current catalog size
- Projects: 26 (Sharp.Shared / Sharp.Core / Sharp.Generator(.Sdk) / Sharp.Extensions.\* / Sharp.Modules.\*)
- Public types: **1197** (of which Source-Generator-emitted: **64**)
- Public methods: 9213
- Namespaces: 54
- `Sharp.Shared` — the main consumer-facing project — covers 1073 types across 21 namespaces

The 64 Source-Generator-emitted types (nested `*.Types` classes produced
for protobuf messages) are summarized in `catalog/indexes/generated-types.md`.

## First-time setup
```bash
git clone --recurse-submodules <this-repo>
```
If you forgot `--recurse-submodules`:
```bash
git submodule update --init --recursive
```

## Updating the catalog
Open a Claude Code session in this repository and say something
like "update the catalog". Claude Code follows the runbook in
`CLAUDE.md` and runs the commands itself — there is intentionally
no shell script or CI automation for this.

## Consuming this catalog from another project
```bash
cd my-plugin
git submodule add <this-repo> refs/modsharp-knowledge
```

Quickest way to wire it into the plugin's `CLAUDE.md` — open Claude Code
in the plugin repo and say:

> Follow `refs/modsharp-knowledge/init.md`

`init.md` is an interactive setup runbook. It asks which preset (Full /
Minimal / Custom) you want, then inserts the corresponding block into
your plugin's `CLAUDE.md` between well-known markers so a later re-run
can update it cleanly.

For the manual path, copy the snippet from `docs/usage.md` by hand.

## Language policy
All hand-written content in this repo — `CLAUDE.md`, `README.md`,
files under `patterns/`, `gotchas.md`, `docs/`, commit messages — is
written in **English**. Please keep additions in English even when the
conversation driving the change happens in another language. The
auto-generated `catalog/` is language-neutral; it reproduces whatever
lives in the source code and XML doc comments upstream.

## License
- Repo scaffolding: MIT
- `external/modsharp/`: AGPL-3.0 (ModSharp itself)
- `catalog/`: derived from ModSharp source, so AGPL-3.0 terms may extend to it
