# Samiyah Knowledge Standard

## Overview

This document defines the official standard for every Knowledge document within the Samiyah AI System.

All files inside the knowledge directory must follow this specification.

The objective is to ensure:

- Consistent document structure
- Efficient AI retrieval
- Dynamic Prompt Assembly
- Low token consumption
- High maintainability
- Future RAG compatibility
- AI Memory compatibility
- Multi-Agent collaboration

Knowledge is considered a long-term business asset.

It should be written once and reused everywhere.

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

One document should describe only one business topic.

Never combine unrelated knowledge.

---

# Standard Metadata

Every Knowledge document should begin with metadata.

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

Metadata allows future AI systems to identify the document without reading the entire file.

---

# Standard Document Structure

## 1. Overview

Brief introduction.

Explain what this knowledge describes.

---

## 2. Business Knowledge

Core reusable business knowledge.

Examples

Company

Factory

Website

Products

SEO

Sales

Markets

---

## 3. Business Rules

Internal company rules.

Standards.

Restrictions.

Things AI must always follow.

---

## 4. Best Practices

Industry recommendations.

Internal experience.

Optimization suggestions.

---

## 5. Keywords

Primary Keywords

Secondary Keywords

Business Keywords

These keywords improve semantic retrieval.

---

## 6. AI Usage Rules

Define

When should AI load this document?

When should AI ignore this document?

Typical business scenarios.

---

## 7. Input

Which tasks require this knowledge?

Examples

Blog Writing

Quotation

Website

SEO

Product Page

Solution Page

Customer Development

Factory Introduction

---

## 8. Output

Which deliverables depend on this knowledge?

Examples

Blog

Product CMS

Quotation

Email

Catalog

Landing Page

Solution Page

Product Specification

---

## 9. Called By

List AI Agents.

Examples

AI Sales Director

SEO Growth Agent

Content Creator Agent

Automation Manager Agent

Product Marketing Agent

Customer Success Agent

---

## 10. Dependencies

Knowledge files usually loaded together.

Example

company-profile.md

brand-guidelines.md

website-structure.md

seo-content-rules.md

---

## 11. Priority

Loading priority.

★★★★★ Critical

★★★★ High

★★★ Medium

★★ Low

★ Optional

Prompt Builder should always load higher-priority knowledge first.

---

## 12. Related Documents

Related files outside Knowledge.

Examples

templates/

playbooks/

workflows/

standards/

agents/

---

## 13. Future Expansion

Reserved.

Examples

RAG

Vector Database

Embeddings

Knowledge Graph

Semantic Search

AI Memory

Retrieval Score

Confidence Score

---

## 14. Version

Version

Status

Owner

Last Updated

---

# Naming Rules

Knowledge filenames must

Use lowercase.

Use hyphens.

Describe only one topic.

Keep names concise.

Examples

company-profile.md

website-structure.md

factory-capability.md

seo-content-rules.md

Bad Examples

knowledge.md

company.md

myfile.md

factory-product.md

---

# Content Rules

Knowledge should contain

Long-term information

Company standards

Business processes

Industry expertise

Manufacturing knowledge

SEO knowledge

Product knowledge

Knowledge should NOT contain

Temporary tasks

Meeting notes

Daily records

Customer records

Draft articles

Personal opinions

Project-specific notes

---

# Duplicate Prevention

Every business rule should exist in only one location.

Never duplicate content.

Instead

Reference the original Knowledge document.

Prompt Builder will assemble multiple documents dynamically.

---

# AI Loading Strategy

AI never loads the entire Knowledge Base.

Workflow

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

Load only the required modules.

Ignore everything else.

---

# Knowledge Loading Priority

Always load in this order

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

This order should remain fixed.

---

# Example

Task

Write a Bathroom Faucet Buying Guide

Prompt Builder loads

★★★★★ company-profile.md

★★★★★ brand-guidelines.md

★★★★★ website-structure.md

★★★★★ seo-content-rules.md

★★★★ product-database.md

★★★★ content-strategy.md

★★ customer-profile.md

Ignored

quotation-rules.md

sales-process.md

market-strategy.md

Only relevant knowledge should be loaded.

---

# Token Optimization Rules

To minimize token consumption

Load only required documents.

Never load duplicate knowledge.

Keep every Knowledge file independent.

Separate reusable rules.

Store facts only once.

Reference instead of copy.

Prompt Builder should remove duplicate instructions automatically.

---

# AI Retrieval Rules

Future retrieval methods may include

Keyword Matching

Metadata Search

Vector Search

Semantic Search

Knowledge Graph

RAG

AI Memory

Hybrid Retrieval

The Knowledge structure should remain compatible with all future retrieval methods.

---

# Future Roadmap

Future versions may introduce

Knowledge Tags

Embedding IDs

Vector IDs

Knowledge Scores

Retrieval Scores

Confidence Scores

Knowledge Ranking

Dependency Detection

Automatic Prompt Assembly

Context Compression

Multi-Agent Knowledge Sharing

AI Memory Integration

---

# Core Philosophy

Write once.

Reuse everywhere.

Avoid duplication.

Load only what is needed.

Optimize every token.

Keep knowledge modular.

Design for long-term growth.

Think like an AI Operating System.

---

# Version

Version: V3.0

Status: Active

Owner: Samiyah AI System

Last Updated: July 2026
