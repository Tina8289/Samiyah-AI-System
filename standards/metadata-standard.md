# Samiyah Metadata Standard

## Overview

This document defines the standard metadata format for all Markdown documents within the Samiyah AI System.

Every document should begin with a metadata section.

Metadata allows AI systems, Prompt Builder, Make automation, GitHub Agents, and future RAG engines to identify documents without reading the entire content.

This standard applies to all directories unless otherwise specified.

---

# Purpose

Metadata enables:

- Faster document retrieval
- Better Prompt Assembly
- Lower token usage
- AI-readable document management
- Future semantic search
- Version control
- Dependency management

---

# Standard Metadata

Every document should begin with the following metadata.

```yaml
id:

title:

type:

category:

priority:

status:

version:

owner:

tags:

called_by:

depends_on:

related_documents:

created_date:

last_updated:
```

---

# Field Definitions

## id

Unique document identifier.

Example

KNOW-0001

TEMP-0008

WORK-0012

AGENT-0003

---

## title

Official document title.

---

## type

Document type.

Allowed values

Documentation

Standard

Knowledge

Template

Playbook

Workflow

Agent

Customer

Market

Product

Asset

---

## category

Top-level folder.

Examples

knowledge

agents

templates

workflows

playbooks

standards

docs

---

## priority

Document loading priority.

★★★★★ Critical

★★★★ High

★★★ Medium

★★ Low

★ Optional

---

## status

Allowed values

Draft

Review

Active

Deprecated

Archived

---

## version

Current version.

Example

1.0

2.1

3.0

---

## owner

Document owner.

Normally

Samiyah AI System

---

## tags

Business keywords.

Examples

SEO

Bathroom

OEM

Quotation

Blog

Factory

---

## called_by

Which AI Agents may load this document.

---

## depends_on

Required documents.

These should usually be loaded together.

---

## related_documents

Additional references.

These are optional.

---

## created_date

Document creation date.

---

## last_updated

Latest update date.

---

# ID Naming Rules

Each category has its own prefix.

Documentation

DOC

Standards

STD

Knowledge

KNOW

Template

TEMP

Playbook

PLAY

Workflow

WORK

Agent

AGENT

Customer

CUST

Market

MARKET

Product

PROD

Assets

ASSET

Examples

DOC-0001

KNOW-0007

PLAY-0013

WORK-0009

---

# Metadata Principles

Metadata should

Be concise.

Remain stable.

Describe the document.

Avoid business content.

Metadata is for AI systems.

The document body is for business knowledge.

---

# AI Loading Rules

Prompt Builder should first read Metadata.

Only if the Metadata matches the current task should the full document be loaded.

This significantly reduces token usage.

---

# Future Compatibility

Metadata is designed for:

OpenAI API

Make Automation

GitHub Agent

Prompt Builder

Vector Database

RAG

Semantic Search

Knowledge Graph

AI Memory

Multi-Agent Collaboration

---

# Example

```yaml
id: KNOW-0003

title: Website Structure

type: Knowledge

category: knowledge

priority: ★★★★★

status: Active

version: 3.0

owner: Samiyah AI System

tags:

- website

- seo

- navigation

called_by:

- SEO Growth Agent

- Content Creator Agent

depends_on:

- company-profile.md

- brand-guidelines.md

related_documents:

- website-structure.md

created_date: 2026-07

last_updated: 2026-07
```

---

# Core Philosophy

Metadata should answer one question:

"Should this document be loaded?"

If the answer is yes,

Prompt Builder loads the document.

If the answer is no,

Ignore it completely.

---

# Version

Version: V1.0

Status: Active

Owner: Samiyah AI System

Last Updated: July 2026
