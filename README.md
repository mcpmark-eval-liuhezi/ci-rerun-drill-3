# ci-rerun-drill-3
Throwaway repo for CI rerun recovery drill (attempt 3)

## CI Recovery Drill

This repository exercises the on-call recovery runbook for flaky CI:

1. A pull request from `drill/flaky-retry` triggers the CI workflow on `.github/workflows/ci.yml`.
2. The check fails deterministically on every attempt.
3. Recovery is rehearsed by retrying the failed jobs of the run, then re-running the entire run.
