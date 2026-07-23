# Samiyah Knowledge Standard

## Overview

This document defines the official standard for all Knowledge documents within the Samiyah AI System.

Every file stored in the `knowledge/` directory must follow this specification.

The purpose of this standard is to ensure:

- Consistent document structure
- Efficient AI retrieval
- Dynamic Prompt Assembly
- Minimal token consumption
- Easy maintenance
- Future RAG compatibility

Knowledge is considered a long-term business asset and should be reusable across all AI Agents.

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

Each document should describe only one business topic.

Never mix multiple unrelated topics in one document.

---

# Standard Document Structure

Every Knowledge document should follow this structure.

## 1. Overview

Brief introduction explaining the purpose of the document.

---

## 2. Business Knowledge

Core business knowledge.

This is the primary content that AI uses.

Examples:

- Company information
- Factory capability
- Product knowledge
- Website architecture
- SEO strategy

---

## 3. Business Rules

Company standards.

Internal rules.

Operational constraints.

Things AI must always follow.

---

## 4. Best Practices

Recommended methods.

Industry best practices.

Internal recommendations.

Lessons learned.

---

## 5. Keywords

Primary Keywords

Secondary Keywords

Business Keywords

These keywords help future AI retrieval and semantic search.

---

## 6. AI Usage Rules

Define how AI should use this document.

Include:

When should it be loaded?

When should it NOT be loaded?

Typical business scenarios.

---

## 7. Input

Specify which tasks require this knowledge.

Examples:

- Blog Writing
- Product Description
- Solution Page
- Quotation
- Customer Development
- Website Content
- SEO
- Factory Introduction

---

## 8. Output

Specify which deliverables this knowledge influences.

Examples:

- Blog
- Product CMS
- Product Specification
- Solution Page
- Quotation
- Email
- Landing Page
- Catalog

---

## 9. Called By

List AI Agents that normally use this knowledge.

Examples:

- AI Sales Director
- SEO Growth Agent
- Content Creator Agent
- Product Marketing Agent
- Automation Manager Agent

---

## 10. Dependencies

List related Knowledge documents.

Examples:

company-profile.md

brand-guidelines.md

website-structure.md

seo-content-rules.md

---

## 11. Priority

Define loading priority.

★★★★★ Critical

★★★★ High

★★★ Medium

★★ Low

★ Optional

The Prompt Builder should always load higher-priority documents first.

---

## 12. Related Documents

List related files outside the Knowledge directory.

Examples:

templates/

playbooks/

workflows/

standards/

agents/

---

## 13. Future Expansion

Reserved for future AI capabilities.

Examples:

- RAG
- Vector Search
- AI Memory
- Embeddings
- Semantic Search

---

## 14. Version

Version

Status

Owner

Last Updated

---

# Naming Rules

Knowledge files should:

- Use lowercase letters
- Use hyphens (-)
- Be short
- Clearly describe one business topic

Good Examples

company-profile.md

website-structure.md

factory-capability.md

seo-content-rules.md

Bad Examples

company.md

knowledge.md

my document.md

factory_and_product.md

---

# Content Rules

Knowledge should contain

- Facts
- Standards
- Long-term knowledge
- Business processes
- Company rules
- Industry expertise

Knowledge should NOT contain

- Temporary notes
- Daily tasks
- Customer records
- Personal opinions
- One-time projects
- Draft content

---

# Duplicate Prevention

Every business rule should exist only once.

Never copy the same rule into multiple documents.

Instead:

Reference the original Knowledge document.

The Prompt Builder combines documents dynamically.

---

# AI Loading Strategy

AI should never load the entire Knowledge Base.

Instead:

Step 1

Understand the user's request.

↓

Step 2

Select the correct AI Agent.

↓

Step 3

Determine required Knowledge.

↓

Step 4

Load only required files.

↓

Step 5

Ignore unrelated Knowledge.

↓

Step 6

Assemble temporary Prompt.

↓

Step 7

Generate output.

This approach minimizes token usage and improves response quality.

---

# Knowledge Loading Priority

The recommended loading order is:

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

This order should remain consistent across the entire AI System.

---

# Example

Task

Write a Bathroom Faucet Buying Guide.

Prompt Builder loads:

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

factory-capability.md

No unnecessary knowledge should be loaded.

---

# Future Roadmap

Future versions may support:

- AI Memory
- Vector Database
- Retrieval Scores
- Metadata
- Embedding IDs
- Knowledge Tags
- Auto Dependency Detection
- Smart Knowledge Ranking
- Semantic Search
- Multi-Agent Knowledge Sharing

The document structure should remain compatible with future AI technologies.

---

# Core Philosophy

Write once.

Reuse everywhere.

Avoid duplication.

Load only what is needed.

Optimize tokens.

Keep knowledge independent.

Think long-term.

---

# Version

Version: V2.0

Status: Active

Owner: Samiyah AI System

Last Updated: July 2026
