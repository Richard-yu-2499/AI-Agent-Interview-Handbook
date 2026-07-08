# 📘 AI Agent Interview Handbook Style Guide

> Documentation Writing Standard  
> Version: v1.0

---

# 1. Purpose

This document defines the writing standards for the **AI Agent Interview Handbook**.

The objectives are:

- Keep all chapters consistent.
- Ensure high-quality technical explanations.
- Build a handbook that can be maintained for many years.
- Make every chapter easy to read and easy to extend.

Every document in this repository should follow this guide.

---

# 2. Core Philosophy

This handbook follows one simple principle:

> **Explain WHY before WHAT, and WHAT before HOW.**

Every technology chapter should answer the following questions:

1. Why did this technology appear?
2. What problem does it solve?
3. How does it work?
4. How is it used in production?
5. What are the common interview questions?

Readers should understand the evolution of AI technologies instead of memorizing APIs.

---

# 3. Chapter Structure

Every chapter should follow the same structure whenever applicable.

```text
1. Introduction

2. Why It Appeared

3. Historical Background

4. Problems It Solves

5. Core Concepts

6. Architecture

7. Internal Workflow

8. Code Examples

9. Enterprise Practice

10. Comparison

11. Common Mistakes

12. Interview Questions

13. Summary
```

Not every chapter requires every section, but the overall organization should remain consistent.

---

# 4. Writing Style

## Explain from first principles

Always explain:

- Why
- Cause
- Design motivation
- Trade-offs

Avoid explaining only APIs.

---

## Progressive learning

Every chapter should follow this learning order:

```text
Concept

↓

Architecture

↓

Implementation

↓

Code

↓

Production Practice
```

Readers should naturally move from theory to engineering.

---

## Use engineering language

Prefer:

- Architecture
- Workflow
- Runtime
- State
- Execution
- Scheduling

Avoid excessive marketing language.

---

# 5. Markdown Rules

## Headings

Use only one H1 heading per file.

Example:

```text
# Chapter

## Section

### Subsection
```

Do not skip heading levels.

---

## Lists

Use unordered lists for concepts.

Use ordered lists for procedures.

Keep nesting depth as small as possible.

---

## Tables

Use tables when comparing technologies.

Example:

| Technology | Purpose |
|------------|---------|
| Prompt | Control model behavior |
| RAG | Provide external knowledge |
| Fine-tuning | Adapt model capability |

---

# 6. Naming Convention

## File names

Use:

```text
lowercase-with-hyphen.md
```

Example:

```text
why-llm.md
function-calling.md
langgraph-runtime.md
```

Do not use:

```text
WhyLLM.md
FunctionCalling.md
```

---

## Directory names

Use:

```text
docs/

01-llm-foundation/

02-prompt-engineering/

03-embedding/

04-rag/
```

Rules:

- Lowercase only.
- Use hyphen.
- Prefix with numbers.

---

# 7. Code Standards

Primary language:

- Python 3.12+

Requirements:

- Clear variable names.
- Small functions.
- Necessary comments.
- Keep examples executable.

Every code example should explain:

- Purpose
- Input
- Output

Avoid meaningless examples.

---

# 8. Diagram Standards

Use Mermaid whenever possible.

Recommended diagrams:

- Architecture Diagram
- Workflow Diagram
- Sequence Diagram
- State Diagram

Every important technology should include at least one architecture diagram.

---

# 9. Technical Explanation Standard

Every technology should be explained in this order.

## Why

Explain why it exists.

Example:

Why Function Calling?

Because LLMs can generate text, but cannot directly execute external functions.

---

## What

Provide a concise definition.

---

## How

Explain:

- Components
- Workflow
- Runtime
- Execution

---

## Production

Explain:

- Real-world usage
- Advantages
- Limitations

---

# 10. Enterprise Practice

Whenever possible, describe production systems instead of toy examples.

Example topics:

- Enterprise Knowledge Agent
- Customer Service Agent
- Coding Agent
- Data Analysis Agent

Discuss:

- Scalability
- Cost
- Security
- Reliability
- Observability

---

# 11. Interview Question Standard

Every chapter should include an interview section.

Recommended structure:

```text
Question

Short Answer

Deep Explanation

Senior-Level Discussion
```

The goal is to help readers answer questions from different interview levels.

---

# 12. Terminology

The first occurrence of a technical term should include both Chinese and English.

Example:

Retrieval-Augmented Generation（检索增强生成，RAG）

Afterward, use:

RAG

Maintain consistent terminology throughout the handbook.

---

# 13. Images

Store all images under:

```text
images/
```

Recommended structure:

```text
images/

architecture/

workflow/

system-design/
```

Image names should describe their contents.

Example:

```text
rag-retrieval-pipeline.png
```

---

# 14. Git Commit Convention

Use Conventional Commit style.

Examples:

```text
docs: add transformer introduction

docs: improve rag chapter

feat: add langgraph example

fix: correct workflow diagram

refactor: reorganize chapter structure
```

---

# 15. Chapter Review Checklist

Before submitting a chapter, verify the following.

## Content

- Explain why the technology appeared.
- Explain the architecture.
- Explain the workflow.
- Provide code examples.
- Include enterprise practice.
- Include interview questions.

## Technical

- Code examples are correct.
- Framework versions are accurate.
- Diagrams are included.

## Writing

- Terminology is consistent.
- Structure is clear.
- No unnecessary repetition.

---

# 16. Quality Principle

Quality is more important than quantity.

Every chapter should answer one question:

> "Will this chapter help readers truly understand the technology?"

If the answer is no, rewrite it.

---

# 17. Long-Term Maintenance

The AI ecosystem changes rapidly.

When updating the handbook:

- Keep principles stable.
- Update framework versions.
- Add new engineering practices.
- Preserve historical context.

The handbook should remain valuable even as specific frameworks evolve.

---

# Version

Current Version: v1.0

Status: Active
