# Scalability and capacity plan

- Identify expensive route and data-loading paths using browser/server profiling.
- Split bundles by route and lazy-load non-critical features.
- Paginate or virtualize large tables and histories.
- Keep API instances stateless and store durable state in shared storage.
- Cache only safe read-heavy responses with explicit invalidation.
- Apply request size limits, timeouts, rate limits, and bounded retries.
- Track p95/p99 latency, frontend bundle size, error rates, DB pool wait, and background queue depth.

## Release gates
- [ ] Reproducible production build passes.
- [ ] Large collections are paginated or virtualized.
- [ ] Failure handling is tested for unavailable dependencies.
- [ ] Measured performance baselines are recorded.

This file is a planning baseline, not a completed load test.
