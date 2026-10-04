---
name: fivetran-create-retrieve-group
description: Create a new group and then retrieve its details.
api: openapi/fivetran-groups-api-openapi.yml
operations:
- createGroup
- getGroup
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/fivetran-groups-api-openapi.yml ; every operationId checked against the contract
---

# fivetran-create-retrieve-group

Create a new group and then retrieve its details.

## Steps

1. 1. Call `createGroup` with the request body fields required to define the group (e.g., name, description).
2. 2. Call `getGroup` with the `groupId` path parameter returned from the create operation.

## Rules

- Auth: Include a Basic Authentication header as defined by the `basicAuth` scheme.
- Idempotency: The `createGroup` operation is not idempotent; repeat calls may create duplicate groups.
