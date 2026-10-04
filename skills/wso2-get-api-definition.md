---
name: wso2-get-api-definition
description: Retrieve an API's details and download its Swagger definition.
api: openapi/wso2-apis-api-openapi.yml
operations:
- getAllAPIs
- getApisByApiId
- getApisByApiIdSwagger
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/wso2-apis-api-openapi.yml ; every operationId checked against the contract
---

# wso2-get-api-definition

Retrieve an API's details and download its Swagger definition.

## Steps

1. 1. Call `getAllAPIs` – no required query parameters; include the `Authorization` header with a Bearer token.
2. 2. Call `getApisByApiId` – path parameter `apiId`; include the `Authorization` header.
3. 3. Call `getApisByApiIdSwagger` – path parameter `apiId`; include the `Authorization` header.

## Rules

- Authentication: Use the OAuth2Security scheme – send an `Authorization: Bearer <token>` header with each request.
- Rate limiting: Bronze tier allows up to 1000 requests per minute; exceeding this returns no specific HTTP error code.
- Idempotency: All three operations are safe GET calls and can be retried without side effects.
