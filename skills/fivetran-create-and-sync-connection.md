---
name: fivetran-create-and-sync-connection
description: Create a new connection and trigger an incremental sync.
api: openapi/fivetran-connections-api-openapi.yml
operations:
- createConnection
- syncConnection
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/fivetran-connections-api-openapi.yml ; every operationId checked against the contract
---

# fivetran-create-and-sync-connection

Create a new connection and trigger an incremental sync.

## Steps

1. 1. Use `createConnection` with required body fields (e.g., `service`, `schema`, `config`).
2. 2. Use `syncConnection` with path parameter `connectionId` returned from step 1.

## Rules

- Auth: Include Basic Auth header as defined by the `basicAuth` scheme.
- Idempotency: `createConnection` is not idempotent; ensure unique identifiers in the request body if needed.
