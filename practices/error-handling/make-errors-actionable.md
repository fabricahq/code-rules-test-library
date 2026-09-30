---
title: Make errors actionable
whenToRead: When writing or reviewing an error message a user or caller will receive.
impact: MEDIUM
impactDescription: Helps people recover from a failure without guessing what went wrong.
tags: errors
---

## Make errors actionable

Explain what failed and what the user or caller can do next. Include relevant context that is safe to disclose.

Instead of "Invalid configuration", say "The configuration is missing a repository URL. Add a repository value under sources.acme-rules."

Do not include secrets, credentials, or private payloads in an error message. When recovery is not possible, explain the limitation rather than suggesting a retry that cannot help.

Check the message against the failure it describes: the explanation should be accurate and the suggested next step should address the cause.
