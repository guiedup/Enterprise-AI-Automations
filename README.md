# 🤖 Enterprise AI Automations (n8n)

**A professional collection of enterprise-grade AI automation workflows built with n8n, LangChain, and LLMs.**

This repository serves as a showcase for complex automation solutions that bridge the gap between business processes and Generative AI. These workflows demonstrate advanced engineering practices in AI orchestration, RAG (Retrieval-Augmented Generation), multimodal processing, and infrastructure monitoring.

![n8n](https://img.shields.io/badge/n8n-Automation-red.svg)
![LangChain](https://img.shields.io/badge/LangChain-Orchestration-blue.svg)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-green.svg)
![Groq](https://img.shields.io/badge/Groq-Llama--3-orange.svg)
![Supabase](https://img.shields.io/badge/Supabase-Vector--DB-blue.svg)

---

## 🏆 Featured Workflows

### 1. [AI Data Anomaly Analyzer](./workflows/ai-data-anomaly-analyzer)
**The "Smart Infrastructure Monitor"**
- **Core Technology**: LangChain AI Agent + Database Tooling.
- **Problem**: Monitoring distributed infrastructure components manually is inefficient and prone to human error.
- **Solution**: An autonomous AI agent that queries telemetry data periodically, analyzes performance metrics (power output, thermal status), detects anomalies using intelligent reasoning, and reports actionable insights via Telegram.

### 2. [Multimodal WhatsApp AI Bot](./workflows/multimodal-whatsapp-ai-bot)
**The "Intelligent Customer Concierge"**
- **Core Technology**: Multimodal LLMs + Chatwoot + WhatsApp API.
- **Problem**: Support bots usually handle only text, failing when users send PDFs or photos.
- **Solution**: A sophisticated bot capable of "seeing" and "reading" attachments. It extracts text from PDFs, analyzes image content, and processes audio, providing a human-like assistance experience directly on WhatsApp.

### 3. [Vector Data Ingestion Agent](./workflows/vector-data-ingestion-agent)
**The "RAG Knowledge Architect"**
- **Core Technology**: Ollama Embeddings + Supabase Vector Store.
- **Problem**: Keeping an AI's knowledge base updated with user interactions is hard.
- **Solution**: A data pipeline that captures user-taught knowledge, generates semantic embeddings (nomic-embed-text), and upserts them into a vector database. It includes a "Refine" mode where the AI improves existing knowledge based on new context.

### 4. [AI Pricing Optimization Engine](./workflows/ai-pricing-optimization-engine)
**The "Financial Intelligence Consultant"**
- **Core Technology**: Logic-heavy LLM Agent + Postgres Persistence.
- **Problem**: Small businesses struggle with profitable pricing and financial health analysis.
- **Solution**: A consultative AI that guides owners through a data-collection journey, calculates operational costs using tool-calling (Calculator), and provides a strategic diagnostic report for business growth.

### 5. [Automated Document Generation Pipeline](./workflows/automated-document-generation-pipeline)
**The "Zero-Paperwork Engineer"**
- **Core Technology**: Outlook Integration + Google Drive/Docs API.
- **Problem**: Technical reports and service documentation take hours to draft from emails and photos.
- **Solution**: Automatically triggers on incoming emails, extracts technical data, copies document templates, injects field photos, and organizes the final documentation in cloud storage, notifying the team instantly.

---

## 🛠️ Tech Stack & Integrations

- **Orchestration**: n8n (Self-hosted)
- **AI Frameworks**: LangChain (within n8n), OpenAI (GPT-4o), Groq (Llama 3.3).
- **Databases**: Supabase (Vector & Auth), PostgreSQL, Redis.
- **Tools**: WhatsApp Business API, Telegram Bot API, Google Workspace, Microsoft Outlook, Chatwoot.
- **Infrastructure**: Docker-compose, Traefik, VPS.

---

## 🚀 How to Use These Workflows

### Prerequisites
1. A running instance of **n8n** (recommended: Docker version).
2. API keys for the respective services (OpenAI, Groq, Supabase, etc.).

### Import Instructions
1. Navigate to a workflow folder (e.g., `workflows/multimodal-whatsapp-ai-bot`).
2. Download the `workflow.json` file.
3. In your n8n dashboard, click **"Import from File"**.
4. Configure your **Credentials** (placeholders like `[API_KEY_REMOVED]` must be replaced with your actual credentials).

---

## 🏗️ Deployment (Infrastructure as Code)

To replicate the production environment used for these workflows, see the [docker](./docker) directory. It includes a `docker-compose.yml` for:
- n8n (Automation hub)
- Chatwoot (Conversational platform)
- PostgreSQL with pgvector (Vector storage)
- Redis (Messaging broker)

---

## 🙋 Contact & Portfolio

**Guilherme Eduardo Pereira** (@guiedup)
- **Full Python Developer | AI Automation & Computer Vision**
- [GitHub Profile](https://github.com/guiedup)
- [LinkedIn](https://www.linkedin.com/in/guilhermeedupereira)
- [Website](https://tivas.com.br)

---

> *Note: All workflows in this repository have been sanitized for security and confidentiality. Production tokens, private IDs, client names, and sensitive webhook URLs have been replaced with placeholders.*
