# AI Data Anomaly Analyzer

## Overview
An autonomous monitoring workflow that uses an AI agent to analyze infrastructure telemetry, detect operational anomalies, and send real-time alerts.

## Business Problem
Operations teams often struggle to manually monitor complex datasets across multiple entities, leading to delayed responses to overheating, performance drops, or communication failures.

## Solution
This workflow runs on a schedule, queries system data from a centralized database (Supabase), asks an LLM agent to reason over the latest telemetry window, structures the findings as JSON, and notifies stakeholders through Telegram.

## Key Capabilities
- Periodic health analysis of distributed systems.
- Detection of zero power output or inactive states.
- Identification of low performance ratios.
- Automated overheating detection based on threshold logic.
- Detection of communication gaps and heartbeat failures.
- Structured AI output for downstream automated remediation.

## Architecture
1. Schedule trigger starts the monitoring cycle.
2. Time window for analysis is dynamically calculated.
3. LangChain agent queries the data source via specialized tools.
4. Agent reasons over component health and entity status.
5. Structured parser returns `hasProblem` and `detectedAnomalies`.
6. Telegram nodes notify the relevant operations groups.

## Tech Highlights
- n8n LangChain Agent node
- Groq chat model (Llama-3 integration)
- Database tool integration (Supabase)
- Structured reasoning and output parsing
- Automated alerting pipeline

## Why It Matters For Portfolio
This workflow demonstrates AI orchestration for industrial and infrastructure monitoring, showcasing tool-using agents, structured reasoning over time-series data, and real-world operational impact.

## Security Note
All sensitive identifiers, client names, entity IDs, and credentials have been sanitized or replaced with generic placeholders.
