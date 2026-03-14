# WASM Module Size Comparison: Rust vs AssemblyScript

**Author:** frontend-team
**Date:** 2026-03-13

## Summary
Measured compiled WASM output sizes for equivalent data processing modules.

## Results
- Rust (wasm-pack): 42KB gzipped
- AssemblyScript: 28KB gzipped
- Rust with wasm-opt -Oz: 31KB gzipped

## Takeaway
Rust WASM output is slightly larger but offers better runtime performance and type safety.
