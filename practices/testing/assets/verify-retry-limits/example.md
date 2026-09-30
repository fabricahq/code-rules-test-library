# Retry limit example

A client configured for three attempts calls a server that always fails. The test asserts that the server saw exactly three requests.

A second test makes the third attempt succeed and asserts that the client returns the result without a fourth request.
