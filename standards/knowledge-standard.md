# Samiyah Knowledge Standard

## Overview

This document defines the official standard for all Knowledge documents within the Samiyah AI System.

Every file inside the `knowledge/` directory must follow this specification.

The objectives are:

- Standardized document structure
- Efficient AI retrieval
- Modular knowledge management
- Dynamic Prompt Assembly
- Low token consumption
- High maintainability
- Future AI compatibility

Knowledge is a long-term business asset.

Write once. Reuse everywhere.

---

# Design Principles

Every Knowledge document must follow these principles.

- Single Responsibility
- Modular
- Reusable
- Independent
- Maintainable
- Expandable
- AI Readable
- Human Readable
- Machine Readable

Each document should describe only one business topic.

Never combine unrelated knowledge.

Every business rule should exist in only one location.

---

# Metadata Standard

Every Knowledge document should begin with the following metadata.

```yaml
id:
title:
category:
priority:
status:
version:
owner:

tags:

called_by:

depends_on:

related_templates:

related_playbooks:

related_workflows:

last_updated:
```

Metadata enables future AI systems to identify and retrieve documents without reading the entire file.

---

# Standard Document Structure

## 1. Overview

Brief introduction.

Explain what this knowledge describes.

---

## 2. Business Knowledge

Reusable business knowledge.

Examples

- Company
- Factory
- Website
- Products
- SEO
- Sales
- Markets

---

## 3. Business Rules

Company standards.

Internal rules.

Restrictions.

Instructions AI must always follow.

---

## 4. Best Practices

Industry recommendations.

Internal experience.

Optimization suggestions.

---

## 5. Keywords

Include:

- Primary Keywords
- Secondary Keywords
- Business Keywords

These improve semantic retrieval.

---

## 6. AI Usage Rules

Define:

- When AI should load this document.
- When AI should ignore this document.
- Typical business scenarios.

---

## 7. Input

Which tasks require this knowledge?

Examples

- Blog Writing
- Product Page
- Solution Page
- Product Specification
- Website
- SEO
- Customer Development
- Factory Introduction
- Quotation

---

## 8. Output

Which deliverables depend on this knowledge?

Examples

- Blog
- Product CMS
- Solution Page
- Product Specification
- Quotation
- Email
- Catalog
- Landing Page

---

## 9. Called By

List the AI Agents that normally use this knowledge.

Examples

- AI Sales Director
- SEO Growth Agent
- Content Creator Agent
- Product Marketing Agent
- Automation Manager Agent

---

## 10. Dependencies

List Knowledge documents commonly loaded together.

Example

- company-profile.md
- brand-guidelines.md
- website-structure.md
- seo-content-rules.md

---

## 11. Priority

Loading priority.

★★★★★ Critical

★★★★ High

★★★ Medium

★★ Low

★ Optional

Prompt Assembly should always load higher-priority knowledge first.

---

## 12. Related Documents

List related documents outside the Knowledge directory.

Examples

- templates/
- playbooks/
- workflows/
- standards/
- agents/

---

# Naming Rules

Knowledge filenames must:

- Use lowercase.
- Use hyphens.
- Describe only one topic.
- Keep names concise.

Examples

- company-profile.md
- website-structure.md
- factory-capability.md
- seo-content-rules.md

Avoid names such as:

- knowledge.md
- company.md
- myfile.md
- factory-product.md

---

# Content Rules

Knowledge should contain:

- Long-term information
- Company standards
- Business processes
- Industry expertise
- Manufacturing knowledge
- SEO knowledge
- Product knowledge

Knowledge should NOT contain:

- Temporary tasks
- Meeting notes
- Daily records
- Customer records
- Draft articles
- Personal opinions
- Project-specific notes

---

# AI Loading Strategy

AI should never load the entire Knowledge Base.

The loading process should follow this sequence:

User Request

↓

Task Classification

↓

Agent Selection

↓

Knowledge Selection

↓

Template Selection

↓

Playbook Selection

↓

Workflow Selection

↓

Prompt Assembly

↓

OpenAI API

↓

Structured Output

Only load the required modules.

Ignore all unrelated documents.

---

# Loading Priority

Always load modules in the following order:

Standards

↓

Agent

↓

Knowledge

↓

Templates

↓

Playbooks

↓

Workflow

↓

Customer Context

↓

Memory

This loading order should remain consistent across the entire system.

---

# Token Optimization Rules

To minimize token consumption:

- Load only required documents.
- Never load duplicate knowledge.
- Keep every Knowledge document independent.
- Store facts only once.
- Reference instead of copy.
- Reuse existing knowledge whenever possible.

Prompt Assembly should automatically eliminate duplicate instructions before sending the final prompt.

---

# Version

Version: V1.0

Status: Active

Owner: Samiyah AI System

Last Updated: July 2026
