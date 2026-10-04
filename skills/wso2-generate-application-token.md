---
name: wso2-generate-application-token
description: Generate an application token using the appropriate endpoint for the application key type or key mapping.
api: openapi/wso2-application-tokens-api-openapi.yml
operations:
- postApplicationsByApplicationIdKeysByKeyTypeGenerateToken
- postApplicationsByApplicationIdOauthKeysByKeyMappingIdGenerateToken
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/wso2-application-tokens-api-openapi.yml ; every operationId checked against the contract
---

# wso2-generate-application-token

Generate an application token using the appropriate endpoint for the application key type or key mapping.

## Steps

1. 1. Call `postApplicationsByApplicationIdKeysByKeyTypeGenerateToken` with the required path parameters `applicationId` and `keyType`, and include the request body as defined in the contract.
2. 2. Call `postApplicationsByApplicationIdOauthKeysByKeyMappingIdGenerateToken` with the required path parameters `applicationId` and `keyMappingId`, and include the request body as defined in the contract.

## Rules

- Authentication: Include an OAuth2 bearer token in the `Authorization` header.
- Rate limiting: Bronze tier allows up to 1000 requests per minute; exceeding this limit results in no specific HTTP error code.
