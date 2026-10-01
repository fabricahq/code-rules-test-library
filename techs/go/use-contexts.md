---
title: Pass contexts to I/O functions
whenToRead: When writing Go functions that do I/O.
impact: MEDIUM
impactDescription: Prevents calls that cannot be cancelled.
---

## Rule

Pass `context.Context` as the first parameter of every function that does I/O. See [the example](assets/use-contexts/example.go) and [the style guide](../../assets/go-style.md).

## Evidence

I/O functions take a context first.
