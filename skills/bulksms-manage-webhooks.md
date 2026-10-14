---
name: bulksms-manage-webhooks
description: Create, view, update, list, and delete webhooks in the BulkSMS API.
api: openapi/bulksms-openapi.yaml
operations:
- webhook.list
- webhook.create
- webhook.show
- webhook.update
- webhook.delete
generated: '2026-10-14'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/bulksms-openapi.yaml ; every operationId checked against the contract
---

# bulksms-manage-webhooks

Create, view, update, list, and delete webhooks in the BulkSMS API.

## Steps

1. 1. Use `webhook.list` – no request body; optional query parameters for pagination if supported.
2. 2. Use `webhook.create` – send JSON body with required fields (e.g., `url`, `event`) as defined in the contract.
3. 3. Use `webhook.show` – provide the webhook `id` path parameter.
4. 4. Use `webhook.update` – provide the webhook `id` path parameter and JSON body with fields to modify.
5. 5. Use `webhook.delete` – provide the webhook `id` path parameter.

## Rules

- Authentication: Include a Basic Auth header (`Authorization: Basic <base64-encoded-credentials>`).
- All endpoints are accessed via the base URL `https://api.bulksms.com/v1`.
