# Contributing

Thanks for your interest in contributing. This document provides guidelines for both humans and AI assistants.

## Getting Started

1. Fork the repository and clone your fork
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Make your changes following project conventions
4. Run tests and lint before submitting

## Development Workflow

- **Branch from `main`** — Keep your branch up to date
- **Small commits** — One logical change per commit
- **Descriptive messages** — Use imperative mood (e.g., "Add user auth" not "Added user auth")

## Code Standards

- Follow the style and patterns already in the codebase
- Add tests for new functionality
- Update documentation when adding features or changing behavior
- See `AGENTS.md` for AI-specific instructions used across tools

## Pull Requests

- Provide a clear description of the change
- Reference any related issues
- Ensure CI passes before requesting review
- Respond to feedback in a timely manner

## Security

- Never commit secrets, API keys, or credentials
- Report security issues privately rather than in public issues
- Use `.env.example` as a template for environment variables
