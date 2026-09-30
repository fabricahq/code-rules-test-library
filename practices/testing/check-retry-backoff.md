---
title: Check retry backoff
whenToRead: When adding or changing a retry delay.
impact: MEDIUM
impactDescription: Prevents synchronized retries from overwhelming a recovering service.
---

## Check retry backoff

Retry delays must grow between attempts. Add a test that records each delay and asserts that it increases.

See the [retry lifecycle](../../assets/retry-lifecycle.md).
