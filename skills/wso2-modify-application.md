---
name: wso2-modify-application
description: Change the owner of an application and then update its settings.
api: openapi/wso2-application-api-openapi.yml
operations:
- postApplicationsByApplicationIdChangeOwner
- updateApplicationSettings
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/wso2-application-api-openapi.yml ; every operationId checked against the contract
---

# wso2-modify-application

Change the owner of an application and then update its settings.

## Steps

1. 1. Call `postApplicationsByApplicationIdChangeOwner` with the required path parameter `applicationId` and the request body containing the new owner details; include the `Authorization` header.
2. 2. Call `updateApplicationSettings` with the required path parameter `applicationId` and the request body containing the new settings; include the `Authorization` header.

## Rules

- Authentication: Provide a valid OAuth2 token in the `Authorization: Bearer <token>` header.
- Rate limiting: Bronze tier allows up to 1000 requests per minute; exceeding this returns no specific HTTP error code.
- Idempotency: Both operations are not guaranteed to be idempotent; callers should ensure they are not repeated unintentionally.
