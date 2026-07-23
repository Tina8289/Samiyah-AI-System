# Samiyah AI System Data Flow

## Overview

This document defines how information flows through the Samiyah AI System.

Instead of relying on one large prompt, the system dynamically assembles only the modules required for the current task.

This modular approach reduces token consumption, improves maintainability, and allows different AI Agents to share the same knowledge base.

---

# Core Workflow

```text
User Request
        │
        ▼
Coordinator Agent
        │
        ▼
Identify Task Type
        │
        ▼
Select Required AI Agent
        │
        ▼
Load Required Knowledge
        │
        ▼
Load Required Templates
        │
        ▼
Load Required Playbooks
        │
        ▼
Assemble Prompt
        │
        ▼
OpenAI API
        │
        ▼
Generate Structured Output
        │
        ▼
Automation Platform
        │
        ▼
Google Sheets
Make
Wix
CRM
GitHub
```

---

# Step 1 – User Request

The process begins when the user submits a request.

Examples:

- Write a blog
- Generate a quotation
- Recommend products
- Develop a distributor
- Create a product specification
- Research a target market

---

# Step 2 – Coordinator Agent

The Coordinator Agent analyzes the request.

Responsibilities:

- Understand user intent
- Classify task type
- Select the correct AI Agent
- Determine required modules

The Coordinator Agent does not generate business content.

---

# Step 3 – AI Agent Selection

Each task is assigned to a specialized AI Agent.

Examples:

- AI Sales Director
- SEO Growth Agent
- Product Marketing Agent
- Content Creator Agent
- Automation Manager Agent

Each Agent has a single responsibility.

---

# Step 4 – Knowledge Loading

Only the knowledge required for the current task is loaded.

Examples:

- Company Profile
- Product Database
- Factory Capability
- Sales Process
- Website Structure
- Market Strategy

Avoid loading unnecessary knowledge.

---

# Step 5 – Template Loading

Load only the required output template.

Examples:

- Blog CMS Template
- Product CMS Template
- Quotation Template
- Solution Page Template

Templates define output format only.

---

# Step 6 – Playbook Loading

Load the business execution guide.

Examples:

- Write Blog
- Prepare Quotation
- Reply RFQ
- Develop Distributor

Playbooks define execution logic.

---

# Step 7 – Prompt Assembly

The Prompt Builder combines:

- AI Agent
- Knowledge
- Templates
- Playbooks

into one temporary prompt.

This prompt exists only for the current task.

---

# Step 8 – OpenAI API

The assembled prompt is sent to the OpenAI API.

The AI generates structured business output according to the loaded modules.

---

# Step 9 – Automation Platform

The generated result is passed to automation tools.

Examples:

- Make
- Google Sheets
- Wix CMS
- CRM
- GitHub

Automation handles publishing, storage, and synchronization.

---

# Data Flow Principles

The system follows these principles:

## Load Only What Is Needed

Reduce token usage.

Avoid unnecessary context.

---

## Reuse Knowledge

Business knowledge should be written once.

Reuse everywhere.

---

## Separate Responsibilities

Agents

Knowledge

Templates

Playbooks

Workflows

should remain independent.

---

## Dynamic Prompt Assembly

Prompts are assembled dynamically.

Avoid creating one large permanent prompt.

---

## Automation First

Whenever possible, repetitive work should be automated.

---

# Future Expansion

Future integrations may include:

- RAG Knowledge Retrieval
- Vector Database
- AI Memory
- ERP
- PIM
- Supplier Management
- Customer Portal
- Analytics Dashboard

These systems will connect through the same data flow without changing the overall architecture.

---

# Version

Version: V1.0

Status: Active

Owner: Samiyah AI System

Last Updated: July 2026
