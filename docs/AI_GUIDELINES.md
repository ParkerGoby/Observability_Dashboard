# AI Agent Guidelines

This document explains how AI agents should use the various rule and instruction files in this project.

## File Overview

| File | Purpose | Used By |
|------|---------|---------|
| `AGENTS.md` | Vendor-neutral instructions for all AI coding assistants | Cursor, Windsurf, Copilot, Claude Code, Aider, and 25+ tools |
| `.cursor/rules/*.mdc` | Cursor-specific rules with scoping (glob, always-on) | Cursor IDE |
| `CONTRIBUTING.md` | Contribution workflow and standards | Contributors and AI assistants |

## Hierarchy

1. **AGENTS.md** — Read by most AI tools automatically. Place in project root for global rules; add nested `AGENTS.md` in subdirectories for directory-specific guidance.
2. **.cursor/rules/** — Cursor reads these when files match the configured globs or when `alwaysApply: true`. More granular than AGENTS.md for Cursor users.
3. **CONTRIBUTING.md** — Referenced when helping with contributions, PRs, or onboarding.

## Best Practices for Maintainers

- **Keep instructions concise** — Under ~150 lines for AGENTS.md; under ~50 lines per .mdc rule
- **Update when patterns change** — Outdated instructions mislead AI agents
- **Use concrete examples** — Code samples work better than abstract descriptions
- **Define boundaries** — ALWAYS / ASK FIRST / NEVER for security-sensitive actions
- **Iterate** — Add rules when you see the AI making repeated mistakes

## For AI Assistants

When working in this project:

1. Read and follow `AGENTS.md` first
2. If using Cursor, apply matching rules from `.cursor/rules/`
3. Use `CONTRIBUTING.md` when helping with contributions
4. When instructions conflict, ask the user
5. Prefer project conventions over generic best practices
