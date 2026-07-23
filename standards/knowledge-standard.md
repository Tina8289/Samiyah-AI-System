# Samiyah Knowledge Standard

## Overview

This document defines the standard structure for every Knowledge document in the Samiyah AI System.

All files inside the `knowledge/` directory must follow this specification.

The objective is to ensure consistency, improve AI retrieval efficiency, reduce duplicate knowledge, and support dynamic Prompt Assembly.

---

# Design Principles

Every Knowledge document should follow these principles:

- Single Responsibility
- Reusable
- Independent
- Maintainable
- Expandable
- AI Readable
- Human Readable

Each document should describe only one business topic.

---

# Standard Document Structure

Every Knowledge document should contain the following sections.

## 1. Overview

Briefly explain what this knowledge is.

---

## 2. Business Knowledge

The main knowledge content.

This is the core information that AI will use.

---

## 3. Business Rules

Define any company rules, standards, or constraints related to this topic.

---

## 4. Best Practices

Describe recommended methods and practical guidance.

---

## 5. AI Usage Rules

Specify how AI should use this knowledge.

Include:

- When to load
- When not to load
- Typical use cases

---

## 6. Called By

List the AI Agents that may load this knowledge.

Examples:

- AI Sales Director
- Content Creator Agent
- SEO Growth Agent
- Product Marketing Agent
- Automation Manager Agent

---

## 7. Dependencies

List other Knowledge files that are commonly loaded together.

Example:

company-profile.md

brand-guidelines.md

website-structure.md

---

## 8. Priority

Assign a loading priority.

★★★★★ Critical

★★★★ High

★★★ Medium

★★ Low

★ Optional

The Prompt Builder should load higher-priority knowledge first.

---

## 9. Related Documents

List related files.

Examples:

templates/

playbooks/

workflows/

standards/

---

## 10. Version

Version

Status

Owner

Last Updated

---

# Naming Rules

Each Knowledge file should:

- Focus on one topic only.
- Avoid combining unrelated knowledge.
- Use lowercase filenames.
- Use hyphens (-) instead of spaces.
- Keep filenames short and descriptive.

Examples:

company-profile.md

factory-capability.md

website-structure.md

---

# Content Rules

Knowledge should contain:

- Facts
- Company standards
- Reusable information
- Long-term business knowledge

Knowledge should NOT contain:

- Temporary tasks
- Daily notes
- Personal opinions
- Customer-specific information
- One-time project content

---

# Duplicate Prevention

A business rule should exist in only one Knowledge document.

If another document requires the same information, reference it instead of copying it.

The Prompt Builder is responsible for combining multiple Knowledge documents during runtime.

---

# AI Loading Strategy

AI should never load the entire Knowledge Base.

Instead, it should:

1. Identify the task.
2. Select the required AI Agent.
3. Load only the relevant Knowledge documents.
4. Ignore unrelated Knowledge.

This minimizes token usage and improves response quality.

---

# Example

Task:

Write a faucet buying guide.

Load:

★★★★★ company-profile.md

★★★★★ brand-guidelines.md

★★★★★ website-structure.md

★★★★★ seo-content-rules.md

★★★★ product-database.md

★★ customer-profile.md

Do NOT load:

quotation-rules.md

sales-process.md

market-strategy.md

---

# Future Expansion

Future versions may include:

- Tags
- Metadata
- Vector Index
- Embedding IDs
- Retrieval Scores
- AI Memory References

These fields will support advanced RAG and semantic search.

---

# Version

Version: V1.0

Status: Active

Owner: Samiyah AI System

Last Updated: July 2026
