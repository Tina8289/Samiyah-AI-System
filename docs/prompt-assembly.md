# Samiyah AI System Prompt Assembly

## Overview

This document defines how prompts are dynamically assembled in the Samiyah AI System.

Instead of storing one huge prompt, the system builds a temporary prompt by loading only the modules required for the current task.

This approach improves maintainability, reduces token usage, and allows every module to be reused across multiple AI Agents.

---

# Why Prompt Assembly?

A traditional prompt may contain thousands of lines of instructions.

As the business grows, maintaining one large prompt becomes difficult.

The Samiyah AI System separates knowledge into reusable modules and assembles them only when needed.

Benefits:

- Lower token consumption
- Faster responses
- Easier maintenance
- Better scalability
- Reusable knowledge

---

# Prompt Assembly Workflow

```text
User Request
        │
        ▼
Coordinator Agent
        │
        ▼
Identify Task
        │
        ▼
Select AI Agent
        │
        ▼
Determine Required Modules
        │
        ├──────────────┐
        ▼              ▼
Knowledge         Templates
        │              │
        ▼              ▼
Playbooks      Standards
        │              │
        └──────┬───────┘
               ▼
      Prompt Builder
               │
               ▼
      Temporary Prompt
               │
               ▼
          OpenAI API
               │
               ▼
      Structured Output
```

---

# Prompt Components

Each prompt consists of independent modules.

Typical modules include:

- Agent
- Knowledge
- Template
- Playbook
- Standards

Only the required modules are loaded.

---

# Example

Task:

Write a bathroom faucet blog.

The system loads:

Agent

- Content Creator Agent

Knowledge

- Company Profile
- Website Structure
- SEO Content Rules
- Product Database

Template

- Blog CMS Template

Playbook

- Write Blog

Standards

- Markdown Writing Standard

Everything is combined into one temporary prompt.

---

# What Is NOT Loaded?

The following modules are ignored:

- Customer Database
- Quotation Rules
- Sales Workflow
- Hotel Project Playbook
- Market Reports

Only relevant information is loaded.

---

# Prompt Builder

The Prompt Builder is responsible for:

- Reading required modules
- Removing duplicate instructions
- Combining files
- Maintaining loading order
- Building one temporary prompt

The Prompt Builder does not generate business content.

---

# Loading Order

Modules are always loaded in the following order:

1. Standards
2. Agent
3. Knowledge
4. Templates
5. Playbooks

This order should remain consistent across all workflows.

---

# Duplicate Prevention

Avoid loading repeated instructions.

If multiple modules contain the same rule:

- Keep one version
- Ignore duplicates

Knowledge should exist in only one location.

---

# Token Optimization

To reduce token usage:

- Load only required modules
- Avoid duplicate knowledge
- Keep modules independent
- Store reusable rules separately
- Assemble prompts dynamically

---

# Future Expansion

Future Prompt Builder may support:

- Vector Search
- RAG Retrieval
- AI Memory
- Customer Context
- Product Context
- Market Context
- Workflow Context

These features will improve prompt quality without increasing prompt size.

---

# Version

Version: V1.0

Status: Active

Owner: Samiyah AI System

Last Updated: July 2026
