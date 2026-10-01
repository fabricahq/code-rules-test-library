---
title: Return errors to callers
whenToRead: When a Go function can fail.
impact: MEDIUM
impactDescription: Prevents silently ignored failures.
---

## Rule

Return errors to the caller instead of logging them and continuing. Wrap each error with context using `fmt.Errorf("doing x: %w", err)`.

## Evidence

Every function that can fail returns an `error`, and callers handle it.
