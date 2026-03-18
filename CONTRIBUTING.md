# Contributing to OpenPRX

Thank you for your interest in contributing to OpenPRX!

## Getting Started

1. Fork the repository
2. Create a feature branch: `git checkout -b feat/my-feature`
3. Make your changes
4. Run checks: `cargo check && cargo clippy && cargo test` (for Rust projects)
5. Commit with a descriptive message
6. Push and open a Pull Request

## Guidelines

- **Rust projects**: Follow the [Rust API Guidelines](https://rust-lang.github.io/api-guidelines/). No `unwrap()`/`expect()` in production code.
- **Go projects**: Follow standard Go conventions. Run `go vet` and `golint`.
- **Frontend**: Use existing component patterns and styling conventions.

## Reporting Issues

- Use GitHub Issues in the relevant repository
- Include steps to reproduce, expected behavior, and actual behavior
- For security issues, see [SECURITY.md](SECURITY.md)

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (Apache-2.0 or MIT).
