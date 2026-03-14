# Rust Coding Standards and Guidelines

**Author:** architecture-team  
**Date:** 2026-03-12

## Error Handling
- Use `anyhow` for application code, `thiserror` for library code
- Never use `.unwrap()` in production code; use `.expect("reason")` only in tests

## Testing
- Unit tests in the same file using `#[cfg(test)]` modules
- Integration tests in `tests/` directory
- Property-based testing with `proptest` for data transformations

## Dependencies
- Pin major versions in Cargo.toml
- Run `cargo audit` in CI pipeline
- Prefer well-maintained crates with >1000 downloads/week

## Code Style
- Follow `rustfmt` defaults (enforced in CI)
- Use `clippy` with `pedantic` lint group
- Document all public APIs with `///` doc comments
