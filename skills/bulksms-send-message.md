---
name: bulksms-send-message
description: Send a new SMS message using the BulkSMS API.
api: openapi/bulksms-openapi.yaml
operations:
- message.send
- message.show
generated: '2026-10-14'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/bulksms-openapi.yaml ; every operationId checked against the contract
---

# bulksms-send-message

Send a new SMS message using the BulkSMS API.

## Steps

1. 1. Use `message.send` with required fields `to`, `body`, and optional `from` in the request body.
2. 2. Optionally retrieve the sent message details with `message.show` using the returned `id` path parameter.

## Rules

- Authentication: Include a Basic Auth header as defined by the `basicAuth` scheme.
- Idempotency: Not applicable; the API does not define an idempotency key for message sending.
