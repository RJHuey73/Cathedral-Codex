# CLAUDE.md

Guidance for Claude Code (claude.ai/code) working in this repository.

## What This Is

**Cathedral-Codex** has no application code. It holds a one-line
`README.md` (`# Cathedral-Codex`), this file, and seven Claude Code slash
commands under `.claude/commands/` (the SFX-ENG-001 Claude Senior
Engineering Persona Suite, installed in #2). There is no source code,
build, CI or tests.

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
├── README.md                  # single line: "# Cathedral-Codex"
├── CLAUDE.md
└── .claude/commands/          # /eng-architect, /eng-audit, /eng-build, /eng-debug,
                               # /eng-frontend, /eng-optimize, /eng-refactor
```

There is no `src/`, no package manifest (no `package.json`, `pyproject.toml`,
`Cargo.toml`, etc.), no CI configuration, and no tests.

The slash commands are copies, not the source. Each names its authoritative
spec in its front matter: `engineering-codex/prompts/claude-senior-engineering-persona-suite.yaml`
in `RJHuey73/Shadowfox-OS-Specification-Repository`. That repository is
**private**: a session or tool without access to it gets a 404, which means
"no access", not "missing". The suite is v1.1.0 and not ratified there.

## Commands

None. There is no build system, package manager, linter, or test suite in
this repository to invoke. The persona suite's own gate linter
(`persona_suite_lint.py`) lives in the spec repository, not here.

## Conventions

None established yet — there is no code to derive conventions from.

## Gotchas

- If you arrive here expecting the CCX/SFX Federation, CANON-336/337, or a
  "YouTube Channel Growth OS" implementation, it is not in this repo as of
  this writing. Check `git log` and the working tree directly rather than
  trusting descriptions from other repositories' documentation, which may be
  aspirational, stale, or describe a different repo than the one actually
  checked out here.
- To change a persona command, change the spec repository first and re-copy;
  an edit made only here drifts from the source the command declares
  authoritative.
- When real content (code, specs, docs) lands in this repo, this file should
  be rewritten from that actual content — not expanded speculatively ahead
  of it.
