# Automated Document Generation Pipeline

## Overview
An automation pipeline that transforms technical events into structured documents with template management and media insertion.

## Business Problem
Drafting technical reports manually is repetitive, error-prone, and slow—especially when information is scattered across emails, images, and various operational systems.

## Solution
This workflow consumes incoming service data, manages sequential document numbering, copies a master template, injects technical data and uploaded images, and organizes final artifacts in Google Drive while notifying stakeholders.

## Key Capabilities
- Email-triggered document automation.
- Google Drive document template duplication and management.
- Sequential numbering and ID tracking logic.
- Document enrichment with dynamic data injection.
- Automated image upload and inline insertion into documents.
- Team notifications through integrated messaging channels.

## Architecture
1. Email trigger (Outlook) ingests the initial request.
2. Markdown and transformation nodes normalize the inbound content.
3. Google Drive nodes locate the latest document for numbering.
4. Master template is copied and renamed based on event context.
5. Technical data and field images are programmatically inserted.
6. Final documents are stored in structured Drive folders.
7. Real-time notifications are sent to the coordination team.

## Tech Highlights
- Microsoft Outlook integration
- Google Drive and Google Docs API automation
- File handling and inline image insertion logic
- Business logic for sequential ID generation
- Document-centric back-office automation patterns

## Why It Matters For Portfolio
This workflow showcases practical enterprise automation: high-volume document generation, office-suite integration, complex file orchestration, and process acceleration for administrative tasks.

## Security Note
All access tokens, private folder IDs, template references, and webhook IDs were sanitized before publication.
