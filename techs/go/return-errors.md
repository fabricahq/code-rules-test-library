---
title: Return errors to the caller
whenToRead: When calling fallible operations.
impact: HIGH
impactDescription: Keep failures visible so callers can respond.
---

# Return errors to the caller

Return a descriptive error when an operation fails. Let the caller decide whether to retry, report, or stop. Never panic in library code.
