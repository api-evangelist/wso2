# Programmatic API Onboarding — WSO2 API Manager

A single-file, zero-dependency Node.js (18+) CLI that reproduces SoundCloud's
`sc-api-auth.mjs` pattern for WSO2 API Manager: register an application / obtain credentials
programmatically instead of clicking through a dashboard, so agents and developers
can onboard at the command line.

- Script: [`wso2-api-auth.mjs`](wso2-api-auth.mjs)
- Run `node wso2-api-auth.mjs --help` for usage and the required environment variables.
- Story / rationale: https://apievangelist.com/2026/07/16/wso2-api-manager-already-speaks-programmatic-onboarding/

Part of the API Evangelist "Programmatic API Onboarding for the Agentic Moment" series.
