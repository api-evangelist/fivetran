---
name: fivetran-create-and-test-webhook
description: Create an account‑level webhook and then test its delivery.
api: openapi/fivetran-webhooks-api-openapi.yml
operations:
- createAccountWebhook
- testWebhook
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/fivetran-webhooks-api-openapi.yml ; every operationId checked against the contract
---

# fivetran-create-and-test-webhook

Create an account‑level webhook and then test its delivery.

## Steps

1. 1. Call `createAccountWebhook` with the request body fields required to define the webhook (e.g., `url`, `events`).
2. 2. Call `testWebhook` with the `webhookId` returned from the previous step to trigger a test delivery.

## Rules

- Authentication: Use Basic Auth (HTTP) in the `Authorization` header.
- No rate‑limit information is provided; handle HTTP responses accordingly.
