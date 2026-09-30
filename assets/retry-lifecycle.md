# Retry lifecycle

1. Attempt the operation.
2. On a retryable failure, wait for the backoff delay.
3. Stop when the attempt count reaches the limit.
