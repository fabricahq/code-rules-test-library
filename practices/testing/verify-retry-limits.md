---
title: Verify retry limits
whenToRead: When adding or changing code that retries a failed operation.
impact: HIGH
impactDescription: Prevents unbounded retries from overloading dependencies.
---

## Verify retry limits

Every retry loop must stop after a fixed number of attempts. Add a test that fails the operation every time and asserts the number of attempts.

See the [retry lifecycle](../../assets/retry-lifecycle.md) for how attempts, delays, and the limit relate, and a [worked example](assets/verify-retry-limits/example.md).

Check that the test counts attempts rather than elapsed time.
