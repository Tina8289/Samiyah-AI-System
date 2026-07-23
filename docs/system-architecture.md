# Samiyah AI System Architecture

## Overview

This document defines the overall architecture of the Samiyah AI System.

It describes the top-level folder structure, system layers, and the responsibilities of each Category.

This document serves as the master blueprint for the entire AI Operating System.

---

# Design Goals

The architecture is designed to achieve the following objectives:

- Modular Design
- Standardized Knowledge Management
- Reusable Prompt Components
- Scalable AI Agents
- Efficient Business Automation
- Easy Maintenance
- Long-term Expandability

Every component within the system should follow these principles.

---

# Top-Level Architecture

```text
Samiyah-AI-System/
│
├── README.md
│
├── docs/
│
├── standards/
│
├── agents/
│
├── knowledge/
│
├── templates/
│
├── playbooks/
│
├── workflows/
│
├── customer-management/
│
├── customers/
│
├── products/
│
├── markets/
│
├── assets/
│
└── archive/
```

---

# Category Responsibilities

## README.md

Project homepage.

Provides a quick introduction, navigation, and links to all major documentation.

---

## docs/

System documentation.

Explains how the AI System is designed and how it works.

---

## standards/

Development standards.

Defines naming conventions, writing rules, and architectural standards.

---

## agents/

AI role definitions.

Each Agent has a single responsibility.

Agents do not store business knowledge.

---

## knowledge/

Business knowledge base.

Stores reusable business knowledge that can be loaded by different Agents.

---

## templates/

Output templates.

Defines standardized output formats for blogs, products, quotations, and other content.

---

## playbooks/

Business execution guides.

Defines how specific business tasks should be completed.

---

## workflows/

Automation workflows.

Describes end-to-end operational processes involving AI and automation platforms.

---

## customer-management/

Customer management rules.

Defines customer numbering, status, scoring, tagging, and follow-up standards.

---

## customers/

Customer database.

Each customer has an independent file for long-term management.

---

## products/

Product knowledge.

Stores reusable product information used by multiple Agents.

---

## markets/

Market knowledge.

Contains country-specific market information, buyer behavior, regulations, and strategies.

---

## assets/

Static resources.

Stores logos, catalogs, images, PDFs, icons, and reusable media files.

---

## archive/

Historical resources.

Stores deprecated files, old templates, and previous versions.

---

# System Layers

```text
Samiyah AI System
│
├── Layer 1：Foundation
│   ├── README.md
│   ├── docs/
│   └── standards/
│
├── Layer 2：AI Intelligence
│   ├── agents/
│   ├── knowledge/
│   ├── templates/
│   └── playbooks/
│
├── Layer 3：Business Operation
│   ├── workflows/
│   ├── customer-management/
│   ├── customers/
│   ├── products/
│   └── markets/
│
└── Layer 4：Resources
    ├── assets/
    └── archive/
```

---

# Architecture Principles

The Samiyah AI System follows these architectural principles.

## Single Responsibility

Each Category has one clear responsibility.

Avoid overlapping responsibilities.

---

## Modular Design

Every module should work independently.

Modules can be combined when needed.

---

## Reusability

Knowledge should be written once and reused across multiple Agents.

Avoid duplicate content.

---

## Lightweight Loading

Only load the Categories required for the current task.

Avoid loading unnecessary information to reduce token consumption.

---

## Scalability

New modules should be added without changing the overall architecture.

Prefer extending existing Categories instead of creating new top-level Categories.

---

## Standardization

All files should follow unified naming, writing, and documentation standards.

---

# Architecture Workflow

```text
User Request
        │
        ▼
Coordinator Agent
        │
        ▼
Select Required Agent
        │
        ▼
Load Knowledge
        │
        ▼
Load Templates
        │
        ▼
Load Playbooks
        │
        ▼
Assemble Prompt
        │
        ▼
OpenAI API
        │
        ▼
Generate Output
        │
        ▼
Google Sheets / Make / Wix / CRM
```

---

# Future Expansion

The architecture is designed for continuous expansion.

Future modules may include:

- AI Memory
- RAG Knowledge Base
- Multi-Agent Collaboration
- API Integrations
- Analytics Dashboard
- Internal Management Tools

These modules should integrate into the existing architecture without changing the top-level structure.

---

# Version

Version: V1.0

Status: Active

Owner: Samiyah AI System

Last Updated: July 2026
