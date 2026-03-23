# CLAUDE.md

This file provides context and guidance for AI assistants (e.g., Claude Code) working in this repository.

## Repository Overview

**Name:** esto-es-craft
**Status:** Early-stage / scaffold repository
**Current content:** Minimal — only a `README.md` exists at the time of writing.

This repository was initialized with a single commit and is ready for a project to be built out.

## Repository Structure

```
esto-es-craft/
├── README.md       # Project title placeholder
└── CLAUDE.md       # This file
```

As the project grows, update this section to reflect the actual directory layout, entry points, and key modules.

## Git Workflow

### Branch Naming

Feature/task branches follow this convention:

```
claude/<short-description>-<session-id>
```

Examples:
- `claude/add-claude-documentation-fPk0X`

Human-created feature branches should use descriptive names (e.g., `feature/user-auth`, `fix/login-bug`).

### Primary Branches

| Branch   | Purpose                              |
|----------|--------------------------------------|
| `main`   | Stable, production-ready code        |
| `master` | Legacy default branch (mirrors main) |

### Commit Messages

Write clear, imperative commit messages:
- Good: `Add user authentication module`
- Good: `Fix null pointer in payment handler`
- Avoid: `stuff`, `WIP`, `fix`

### Push Instructions

Always use `-u` to set the upstream tracking branch:

```bash
git push -u origin <branch-name>
```

If push fails due to network errors, retry with exponential backoff (2s, 4s, 8s, 16s — max 4 retries).

## Development Setup

> No build system, package manager, or language tooling has been configured yet. Update this section when the project stack is chosen.

Typical setup steps to document here once established:
- How to install dependencies
- How to run the project locally
- Required environment variables

## Testing

> No test framework has been configured yet. Update this section when tests are added.

Document here:
- How to run tests (`npm test`, `pytest`, `cargo test`, etc.)
- Where test files live
- Any coverage requirements

## Linting & Formatting

> No linting or formatting tools configured yet. Update this section when tooling is added.

## Key Conventions

As conventions are established in this project, record them here. Examples to cover:
- File naming style (camelCase, snake_case, kebab-case)
- Module/package structure
- Error handling patterns
- API design conventions

## Updating This File

Keep CLAUDE.md current as the project evolves:
- Add new sections when major tooling is introduced (CI/CD, Docker, databases, etc.)
- Update the directory structure diagram when the layout changes significantly
- Document non-obvious decisions and the reasoning behind them
