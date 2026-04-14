# Vector Data Ingestion Agent

## Overview
A workflow designed to manage long-term AI knowledge through vector storage, semantic retrieval, and iterative knowledge refinement.

## Business Problem
Custom AI assistants become weak when knowledge is not persisted, updated, or retrievable in a semantic way.

## Solution
This workflow classifies user input, stores relevant knowledge into a vector store, updates prior knowledge when needed, and supports retrieval-augmented responses for future conversations.

## Key Capabilities
- Chat-triggered AI training flow.
- Knowledge classification between behavioral rules and factual knowledge.
- Supabase vector store integration.
- Embedding generation with Ollama.
- Retrieval-as-tool for contextual memory.
- Knowledge refinement and update workflows.

## Architecture
1. User input enters through chat trigger.
2. Session state is checked in Supabase.
3. Mode switching controls training vs testing.
4. AI trainer classifies knowledge.
5. AI KNOW stores retrievable content in vector DB.
6. AI FEEL updates behavioral/system instructions.
7. Test mode validates the trained assistant.

## Tech Highlights
- LangChain agents inside n8n
- Supabase vector storage
- Ollama embeddings
- Multi-agent style prompt architecture
- Memory windows and tool routing

## Why It Matters For Portfolio
This is a strong RAG-oriented workflow showing that AI systems need storage, retrieval, updating, and instruction tuning—not only prompts.

## Security Note
Webhook IDs and private references were sanitized before publishing.
