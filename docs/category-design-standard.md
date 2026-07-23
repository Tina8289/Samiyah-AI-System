---
name: Category Design Standard

description:
Defines the design principles for every Category in the Samiyah AI System.

version: 1.0

---

# Category Design Standard


## Purpose


Every Category has one clear responsibility.

Do not mix unrelated content.


Each Category answers four questions:


1. What is its purpose?

2. What does it contain?

3. Who uses it?

4. When should it be used?



---

# Standard Structure


Every Category should include the following sections.


## Purpose


Explain the responsibility of this Category.


Keep it short and clear.



---

## Contents


Describe what belongs here.


Only include files that match the purpose.


Do not duplicate files from other Categories.



---

## Used By


List which Agents or workflows normally use this Category.


Example:


AI Sales Director

Content Creator Agent

Automation Manager Agent



---

## When To Use


Describe the situations where this Category should be loaded.


Example:


Writing blog articles

Preparing quotations

Analyzing customers

Generating product pages



---

# Design Principles


## One Responsibility


Each Category should have only one responsibility.


Avoid overlapping with other Categories.



---

## Reusable


Information should be reusable.


Do not copy the same content into multiple Categories.



---

## Lightweight


Load only what is required for the current task.


Never load the whole system if only one Category is needed.



---

## Easy To Expand


New files should fit naturally into the existing Category.


If not,

create a new Category instead of forcing unrelated files together.



---

# Category Relationships


Categories work together,

but remain independent.


Example:


Agents

↓

Call Knowledge


↓

Call Templates


↓

Call Playbooks


↓

Generate Output



---

# Goal


Build a modular AI operating system that is:

Simple

Scalable

Reusable

Easy to maintain
