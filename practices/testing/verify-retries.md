---
title: Verify retries
whenToRead: When adding or changing code that retries a failed operation or its delays.
impact: HIGH
impactDescription: Prevents retries from overloading a service.
---

## Verify retries

Test every retry policy: assert that delays grow between attempts and include jitter.

See the [retry lifecycle](../../assets/retry-lifecycle.md).
