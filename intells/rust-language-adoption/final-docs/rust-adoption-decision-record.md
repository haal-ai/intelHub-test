# ADR: Rust Adoption for CLI Tooling and WebAssembly

**Status:** Accepted  
**Date:** 2026-03-10  
**Valid Until:** 2027-03-10

## Context
We need a systems programming language for CLI tools and WebAssembly modules. Current Node.js implementations have performance and distribution challenges.

## Decision
Adopt Rust as the primary language for:
- All new CLI tools and developer utilities
- WebAssembly modules for browser and edge compute
- Performance-critical backend services (case-by-case)

## Consequences
- **Positive:** Better performance, smaller binaries, memory safety guarantees
- **Negative:** Steeper learning curve, smaller talent pool, longer initial development time
- **Mitigations:** Dedicated onboarding program, Rust champions in each team, shared libraries
