# Multimodal WhatsApp AI Bot

## Overview
A production-grade WhatsApp bot that handles text, image, PDF, and support-routing flows using AI and external integrations.

## Business Problem
Most messaging bots fail when customers send attachments, mixed content, or need integration with support systems like Chatwoot.

## Solution
This workflow classifies incoming WhatsApp content, extracts PDF text, processes image-related inputs, bridges conversations with support tooling, and uses AI to answer or route messages.

## Key Capabilities
- WhatsApp-triggered conversational automation.
- PDF extraction and text-based processing.
- Image-aware message handling.
- Chatwoot API integration.
- AI-generated replies.
- Lead/customer routing and notification flows.

## Architecture
1. WhatsApp trigger receives inbound message.
2. Input is classified by type.
3. PDFs are parsed and transformed into text context.
4. Images and plain messages are normalized.
5. AI nodes generate response or support actions.
6. Chatwoot/HTTP nodes send updates and messages.
7. Notifications and logging complete the cycle.

## Tech Highlights
- WhatsApp Business API nodes
- Chatwoot API orchestration
- LLM response generation
- Multimodal preprocessing
- Human-support escalation paths

## Why It Matters For Portfolio
This workflow is highly relevant for AI automation jobs because it combines messaging, AI, support tooling, document extraction, and production workflow logic.

## Security Note
Access tokens, notes, static chat IDs, and webhook references were removed.
