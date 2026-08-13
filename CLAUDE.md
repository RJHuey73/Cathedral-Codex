# CLAUDE.md

Guidance for Claude Code (claude.ai/code) working in this repository.

## What This Is

**Cathedral-Codex** is, as of this writing, an essentially empty repository.
The entire contents are a single `README.md` with just the title
(`# Cathedral-Codex`) — no source code, no configuration, no docs beyond
that one line.

A sibling repo's documentation (`ske-shadowfox`) references a "CCX/SFX
Federation" involving this repo (CANON-336/337, a "YouTube Channel Growth
OS"). **That architecture is not present here.** Nothing in this repository
— no code, no config, no docs — currently substantiates those claims. Do
not assume federation code, CANON references, or a Growth OS exist in this
repo; verify against actual repo contents (`ls -la`, `git log`) before
relying on external descriptions of what this repo contains.

## Layout

```
Cathedral-Codex/
└── README.md   # single line: "# Cathedral-Codex"
```

There is no `src/`, no package manifest (no `package.json`, `pyproject.toml`,
`Cargo.toml`, etc.), no CI configuration, and no tests.

## Commands

None. There is no build system, package manager, linter, or test suite in
this repository to invoke.

## Conventions

None established yet — there is no code to derive conventions from.

## Gotchas

- If you arrive here expecting the CCX/SFX Federation, CANON-336/337, or a
  "YouTube Channel Growth OS" implementation, it is not in this repo as of
  this writing. Check `git log` and the working tree directly rather than
  trusting descriptions from other repositories' documentation, which may be
  aspirational, stale, or describe a different repo than the one actually
  checked out here.
- When real content (code, specs, docs) lands in this repo, this file should
  be rewritten from that actual content — not expanded speculatively ahead
  of it.
