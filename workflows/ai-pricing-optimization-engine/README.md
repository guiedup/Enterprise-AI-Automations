# AI Pricing Optimization Engine

## Overview
A consultative AI workflow that helps dentistry clinics evaluate pricing, profitability, and business performance.

## Business Problem
Many small clinics do not know their true service profitability, hourly cost structure, or ideal revenue targets.

## Solution
This workflow conducts a guided conversation, stores lead memory, calculates operational metrics with tool calling, classifies commercial potential, and generates a strategic analysis for the clinic owner.

## Key Capabilities
- Conversational lead qualification.
- Persistent business memory in Postgres.
- Calculator-assisted financial reasoning.
- Pricing and margin analysis.
- Follow-up classification and export flows.
- Strategic diagnostic messaging.

## Architecture
1. Chat trigger starts the consultation.
2. Existing lead data is loaded from Postgres.
3. AI memory is summarized and updated.
4. Main AI agent collects operational and financial inputs.
5. Calculator tool supports pricing analysis.
6. Results are stored and classified.
7. Export/download endpoints generate reporting outputs.

## Tech Highlights
- Postgres persistence
- Tool-calling for deterministic calculations
- Long-term lead memory
- AI-driven business diagnostics
- Webhook-based export flow

## Why It Matters For Portfolio
This workflow proves business-facing AI engineering: memory, analytics, prompt architecture, qualification logic, and measurable commercial use cases.

## Security Note
An exposed API key found in node notes was removed, along with webhook IDs and other sensitive references.
