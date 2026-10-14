---
name: bulksms-blocked-numbers-manage
description: Manage blocked numbers by listing existing entries and adding new ones.
api: openapi/bulksms-openapi.yaml
operations:
- blocked.list
- blocked.create
generated: '2026-10-14'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/bulksms-openapi.yaml ; every operationId checked against the contract
---

# bulksms-blocked-numbers-manage

Manage blocked numbers by listing existing entries and adding new ones.

## Steps

1. 1. Use `blocked.list` with no additional fields or headers beyond the required Basic Auth header.
2. 2. Use `blocked.create` with the request body field `number` (the phone number to block) and the required Basic Auth header.

## Rules

- Auth: Include a Basic Auth header as defined by the `basicAuth` scheme.
- Idempotency: Not applicable; the `blocked.create` operation does not specify an idempotency key.
