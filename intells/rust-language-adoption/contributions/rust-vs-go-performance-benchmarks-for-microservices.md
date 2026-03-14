# Rust vs Go Performance Benchmarks for Microservices

**Author:** team-perf  
**Date:** 2026-02-20

## Summary
Comparative benchmarks of Rust (Actix-web) and Go (Gin) for common microservice workloads.

## Results

| Workload | Rust (Actix) | Go (Gin) | Delta |
|---|---|---|---|
| HTTP JSON response (p99) | 1.2ms | 3.8ms | -68% |
| gRPC unary call (p99) | 0.8ms | 2.1ms | -62% |
| JSON serialize 10K objects | 4ms | 12ms | -67% |
| Memory under 1K concurrent | 18MB | 42MB | -57% |

## Conclusion
Rust shows significant performance advantages for latency-critical services. Go remains more productive for simpler CRUD services where latency is not the primary concern.
