---
title: Test changed behavior
whenToRead: When adding or changing externally visible behavior.
impact: HIGH
impactDescription: Prevents behavior changes from silently breaking existing use cases.
tags: testing
---

## Test changed behavior

When a change alters behavior that a caller or user relies on, add or update a test for that outcome.

For example, if a discount changes an order's total, assert the resulting total rather than which private helper was called.

Run the relevant tests before you consider the change complete.
