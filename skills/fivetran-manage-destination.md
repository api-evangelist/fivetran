---
name: fivetran-manage-destination
description: Create, retrieve, update, and delete a destination.
api: openapi/fivetran-destinations-api-openapi.yml
operations:
- createDestination
- getDestination
- updateDestination
- deleteDestination
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/fivetran-destinations-api-openapi.yml ; every operationId checked against the contract
---

# fivetran-manage-destination

Create, retrieve, update, and delete a destination.

## Steps

1. 1. Use `createDestination` with the request body fields required to define a new destination.
2. 2. Use `getDestination` with the path parameter `destinationId` to retrieve the created destination.
3. 3. Use `updateDestination` with the path parameter `destinationId` and the request body fields to modify the destination.
4. 4. Use `deleteDestination` with the path parameter `destinationId` to remove the destination.

## Rules

- Authentication: Include a Basic Auth header as defined by the `basicAuth` scheme.
- Idempotency: `createDestination` and `updateDestination` are not idempotent; repeat calls may create duplicate resources or apply additional changes.
- Pagination: Not applicable; these endpoints operate on single resources.
- Errors: The API returns standard HTTP error codes; on rate‑limit exhaustion no specific limit is defined.
