# Architecture Documentation

## Overview
This Multi-Agent implements DSAR Precedent Finder for evidence for Legal & Compliance use cases.

## Components
1. **Request Intake**: Collect, validate and normalize emails from Records; attach a runId and timestamp for traceability.
2. **Delegate**: Execute delegate phase for the Multi-Agent pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Handoff**: Execute handoff phase for the Multi-Agent pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Entity Extraction**: Entity Extraction across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Policy Check**: Policy Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Review Routing**: Review Routing across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Classification**: Classification across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
8. **Ingestion**: Ingestion across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
9. **Privilege Log**: Assemble final payload with status, artifacts, KPIs and audit trail; store to DMS; return response JSON for the client.

## Data Flow
- Input: Request Intake
- Processing: 9 sequential steps
- Output: Privilege Log
