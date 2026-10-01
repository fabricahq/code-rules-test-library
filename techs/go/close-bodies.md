---
title: Close response bodies
whenToRead: When making HTTP requests in Go.
impact: MEDIUM
impactDescription: Prevents leaked connections.
---

## Rule

Close every HTTP response body with `defer resp.Body.Close()` right after checking the error.

## Evidence

Each successful request is followed by a deferred close of its body.
