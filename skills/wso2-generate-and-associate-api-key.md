---
name: wso2-generate-and-associate-api-key
description: Generate an API key for a specific API and associate it with an application.
api: openapi/wso2-api-keys-api-openapi.yml
operations:
- generateApiBoundApiKey
- associateAPIKeyToApp
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/wso2-api-keys-api-openapi.yml ; every operationId checked against the contract
---

# wso2-generate-and-associate-api-key

Generate an API key for a specific API and associate it with an application.

## Steps

1. 1. Call `generateApiBoundApiKey` with the required path parameter `apiId` and request body fields as defined in the contract.
2. 2. Call `associateAPIKeyToApp` with path parameters `applicationId` and `keyType`, and include the generated API key in the request body as specified.

## Rules

- Auth: Include an `Authorization: Bearer <access_token>` header using the OAuth2Security scheme.
- Rate limit: Bronze tier – 1000 requests per minute; on exhaustion the service returns no specific HTTP error code.
- Idempotency: POST operations are not idempotent; avoid duplicate calls.
