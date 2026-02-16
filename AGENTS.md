# Microservice Project — AI Agent Instructions

This file provides instructions for AI coding assistants (Cursor, Copilot, Windsurf, Claude Code, etc.). Follow these rules when working in this project.

## Build & Test Commands

- Run tests: `pytest` or `npm test` (depending on service)
- Lint/format: `ruff check .` or `npm run lint`
- Type-check: `mypy .` or `npm run typecheck`
- Start development: See individual service READMEs

## Code Style & Conventions

- Follow existing patterns in the codebase
- Prefer explicit over implicit; avoid magic values
- Use meaningful variable and function names
- Document public APIs and non-obvious logic

## Project Structure

- Each microservice lives in its own directory with its own dependencies
- Shared utilities go in a common module
- Config and secrets: use environment variables, never hardcode

## Security Boundaries

- **ALWAYS**: Run tests before committing; use `.env.example` as template, never commit `.env`
- **NEVER**: Commit secrets, API keys, or credentials; modify production config without review
- **ASK FIRST**: Before changing auth flows, database schemas, or external integrations

## Git Workflow

- Create feature branches from `main`; do not commit directly to `main`
- Write clear commit messages; reference issues when applicable
- Keep changes focused—one logical change per commit

## When in Doubt

- Prefer consistency with existing code over "best practice" from scratch
- If conventions conflict, ask the user
- Preserve backward compatibility unless explicitly changing a public API
