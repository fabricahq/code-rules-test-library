---
title: Verify retry limits
whenToRead: When adding or changing retries.
impact: MEDIUM
impactDescription: Prevents unbounded retries.
---

## Rule

Test that every retry policy stops after its limit. Use a fake clock. See [the retry lifecycle](../../assets/retry-lifecycle.md).

## Evidence

A test exercises the limit for each retry policy.
