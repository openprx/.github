# Contributing to OpenPRX

Thank you for your interest in contributing! This guide applies to all repositories under the OpenPRX organization.

## Getting Started

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-change`
3. Make your changes
4. Run tests (if applicable)
5. Commit with a clear message: `git commit -m "feat: add feature X"`
6. Push and open a Pull Request

## Commit Convention

We follow [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` — New feature
- `fix:` — Bug fix
- `docs:` — Documentation only
- `refactor:` — Code change that neither fixes a bug nor adds a feature
- `test:` — Adding or updating tests
- `chore:` — Maintenance tasks
- `ci:` — CI/CD changes

## Pull Requests

- Keep PRs focused and small
- Include a clear description of what and why
- Link related issues
- Ensure CI passes

## Development Setup

Each repository has its own setup instructions in its README. General requirements:

- **Rust projects** (OpenPR, PRX, prx-memory): Rust 1.75+, cargo
- **Site**: Node.js 22+, npm

## Code Style

- Rust: `cargo fmt` and `cargo clippy`
- TypeScript/JS: project-specific linting

## License

By contributing, you agree that your contributions will be licensed under the Apache License 2.0.
