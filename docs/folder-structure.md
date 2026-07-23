# Samiyah AI System Folder Structure

## Overview

This document defines the purpose, contents, usage, and relationships of every top-level Category in the Samiyah AI System.

Each Category has a single responsibility.

Avoid placing unrelated content into the same Category.

---

# README.md

## Purpose

Project homepage.

Provide project introduction and documentation navigation.

## Contents

- Project introduction
- Quick start
- Documentation links

## Used By

Everyone

## When To Use

The first document to read after entering the project.

---

# docs/

## Purpose

Store all project documentation.

## Contents

- System Overview
- System Architecture
- Folder Structure
- Data Flow
- Prompt Assembly
- Automation Roadmap

## Used By

Developers

AI Engineers

Future Contributors

## When To Use

Understand how the entire AI System is designed.

---

# standards/

## Purpose

Store development standards.

## Contents

- Category standards
- File naming rules
- Folder naming rules
- Markdown writing standards
- Prompt writing standards

## Used By

All developers

All AI Agents

## When To Use

Before creating new files or modifying existing structures.

---

# agents/

## Purpose

Store AI role definitions.

## Contents

Each file defines one AI Agent.

Examples:

- AI Sales Director
- SEO Growth Agent
- Content Creator Agent

## Used By

Coordinator Agent

Automation Workflows

## When To Use

Whenever an AI role needs to perform a task.

---

# knowledge/

## Purpose

Store reusable business knowledge.

## Contents

- Company information
- Product knowledge
- Factory capability
- Website structure
- SEO rules
- Sales knowledge

## Used By

All AI Agents

## When To Use

Whenever business knowledge is required.

---

# templates/

## Purpose

Store standardized output formats.

## Contents

- Blog Template
- Product Template
- Solution Template
- Quotation Template

## Used By

Content Agents

Sales Agents

## When To Use

Whenever structured output is required.

---

# playbooks/

## Purpose

Store business execution guides.

## Contents

- Blog Writing
- Quotation Preparation
- Customer Development
- Product Recommendation

## Used By

Business Agents

## When To Use

When executing complete business tasks.

---

# workflows/

## Purpose

Store automation workflows.

## Contents

- Make Automation
- Wix Publishing
- Lead Generation
- Product Upload

## Used By

Automation Manager Agent

## When To Use

When executing automated business processes.

---

# customer-management/

## Purpose

Store customer management standards.

## Contents

- Customer ID Rules
- Customer Status
- Customer Scoring
- Customer Tags
- Follow-up Rules

## Used By

Sales Agents

CRM Automation

## When To Use

Whenever customer information is managed.

---

# customers/

## Purpose

Store customer records.

## Contents

One file per customer.

## Used By

Sales Team

Sales Agents

## When To Use

Managing customer history.

---

# products/

## Purpose

Store product knowledge.

## Contents

- Toilets
- Basins
- Faucets
- Showers
- Accessories

## Used By

Product Agents

Sales Agents

Content Agents

## When To Use

Whenever product information is needed.

---

# markets/

## Purpose

Store market knowledge.

## Contents

- Europe
- USA
- Middle East
- Bangladesh
- Indonesia

## Used By

Sales Agents

Marketing Agents

## When To Use

When developing different international markets.

---

# assets/

## Purpose

Store reusable resources.

## Contents

- Logos
- Images
- Catalogs
- PDFs

## Used By

Everyone

## When To Use

Whenever static resources are required.

---

# archive/

## Purpose

Store historical resources.

## Contents

- Deprecated files
- Old prompts
- Old templates

## Used By

Developers

## When To Use

When retiring old content without deleting history.

---

# Folder Design Principles

Every Category follows these principles.

- Single Responsibility
- Modular Design
- Reusable Content
- Easy Maintenance
- Easy Expansion
- Standardized Structure

Future Categories should only be created when absolutely necessary.
