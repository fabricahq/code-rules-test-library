---
title: Wrap errors with context
whenToRead: When returning an error received from another call.
impact: MEDIUM
impactDescription: Makes failures traceable to the operation that caused them.
---

## Wrap errors with context

When you return an error you received from another call, add the operation you were attempting, such as "load config: open file: permission denied".

Keep the original error available to callers that inspect it.

In Go, use `fmt.Errorf("load config: %w", err)` so callers can still use `errors.Is`.

Check each returned error: a reader should be able to tell which operation failed without a stack trace.
