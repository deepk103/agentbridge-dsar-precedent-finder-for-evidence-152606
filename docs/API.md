# API Documentation

## Endpoints
### Request Intake
- **Description**: Collect, validate and normalize emails from Records; attach a runId and timestamp for traceability.
- **Type**: Processing

### Delegate
- **Description**: Execute delegate phase for the Multi-Agent pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Handoff
- **Description**: Execute handoff phase for the Multi-Agent pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Entity Extraction
- **Description**: Entity Extraction across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Policy Check
- **Description**: Policy Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Review Routing
- **Description**: Review Routing across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Classification
- **Description**: Classification across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Ingestion
- **Description**: Ingestion across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Privilege Log
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to DMS; return response JSON for the client.
- **Type**: Processing
