# 📚 AI Agent Interview Handbook

> From LLM to AI Agent System Design

本文件是整个 AI Agent Handbook 的学习导航。

推荐按照章节顺序学习。

---

# Part 01 · LLM Foundation

> Understanding the brain behind AI Agents.

AI Agent 的核心能力来自 Large Language Models。

本部分回答：

- LLM 为什么出现？
- Transformer 为什么重要？
- GPT 为什么成功？
- LLM 有哪些能力边界？

---

## 01 LLM 基础

### 01.1 AI 发展历史

- 从传统机器学习到深度学习
- 神经网络的发展
- 深度学习革命
- 大语言模型时代

---

### 01.2 Transformer

- 为什么 RNN 存在瓶颈
- Attention 机制
- Self-Attention
- Transformer Architecture

---

### 01.3 GPT 系列

- GPT-1
- GPT-2
- GPT-3
- GPT-4
- GPT-4o
- Reasoning Model

---

### 01.4 LLM 核心机制

- Token
- Tokenizer
- Context Window
- KV Cache
- Temperature
- Sampling

---

### 01.5 LLM 能力与限制

- Language Understanding
- Reasoning
- Hallucination
- Knowledge Cutoff
- Long Context Limitation

---

### 01.6 高频面试题

- Transformer 为什么替代 RNN？
- GPT 为什么具有涌现能力？
- LLM 为什么会产生幻觉？


---

# Part 02 · Prompt Engineering

> Teaching LLM how to think and respond.

---

## 02 Prompt Engineering

### 02.1 Prompt 基础

- Prompt 是什么
- 为什么需要 Prompt
- Prompt 与 Programming 的区别

---

### 02.2 Prompt 技术

- Zero-shot
- Few-shot
- Role Prompting
- Chain of Thought
- Self Consistency
- Tree of Thought

---

### 02.3 Prompt Engineering 实践

- System Prompt
- Developer Prompt
- Instruction Design
- Prompt Template

---

### 02.4 面试问题

- Prompt 为什么有效？
- Prompt Engineering 会消失吗？


---

# Part 03 · Knowledge Augmentation

> Giving LLM external knowledge.

---

# 03 Embedding

内容：

- Vector Representation
- Embedding Model
- Similarity Search
- Vector Database


---

# 04 RAG

内容：

- 为什么需要 RAG
- RAG Architecture
- Document Pipeline
- Retrieval
- Chunk Strategy
- Rerank
- Hybrid Search
- Advanced RAG


---

# Part 04 · LLM Action Capability

> From answering questions to taking actions.

---

# 05 Function Calling

内容：

- 为什么出现 Function Calling
- LLM Tool Interface
- Schema Design
- Function Execution


---

# 06 Tool Calling

内容：

- Tool Concept
- Tool Runtime
- Tool Management
- Tool Security


---

# Part 05 · Agent Framework

> Building intelligent workflows.

---

# 07 LangChain

内容：

- LangChain Philosophy
- LCEL
- Chain
- Agent
- Tool
- Memory


---

# 08 LangGraph

内容：

- Why LangGraph
- Graph Architecture
- Node
- Edge
- Runtime
- Checkpoint


---

# 09 StateGraph

内容：

- State Design
- Reducer
- Graph Execution
- Persistence


---

# 10 ReAct

内容：

- Reasoning + Acting
- Thought
- Action
- Observation
- Agent Loop


---

# Part 06 · Agent Memory & Workflow

---

# 11 Memory

内容：

- Short Term Memory
- Long Term Memory
- Vector Memory
- Conversation Memory


---

# 12 Workflow

内容：

- Workflow vs Agent
- Deterministic Workflow
- Agent Workflow
- Human-in-the-loop


---

# Part 07 · Agent Communication

> From single Agent to Agent Ecosystem.

---

# 13 MCP

内容：

- Why MCP
- MCP Architecture
- MCP Server
- MCP Client
- MCP Protocol


---

# 14 Multi-Agent

内容：

- Why Multi-Agent
- Agent Collaboration
- Supervisor Pattern
- Worker Pattern
- Debate Pattern


---

# 15 A2A

内容：

- Why Agent Communication Protocol
- A2A Architecture
- Agent Discovery
- Agent Message
- Agent Collaboration


---

# Part 08 · Enterprise AI Agent

---

# 16 Agent Architecture

内容：

- Enterprise Agent System
- Agent Platform
- Agent Infrastructure


---

# 17 Agent Design Pattern

内容：

- Planner Agent
- Router Agent
- Executor Agent
- Reviewer Agent


---

# 18 Agent Performance

内容：

- Latency Optimization
- Cost Optimization
- Evaluation
- Observability


---

# 19 Agent Security

内容：

- Prompt Injection
- Data Security
- Tool Security
- Permission Management


---

# Part 09 · Interview Handbook

---

# 20 高频面试题

包含：

- LLM 面试题
- RAG 面试题
- Agent 面试题
- LangGraph 面试题
- MCP 面试题
- System Design 面试题


---

# Appendix

## A. Code Examples

- Python
- LangChain
- LangGraph
- MCP
- A2A


---

## B. System Design Cases

案例：

- Enterprise Knowledge Agent
- Customer Service Agent
- Coding Agent
- Data Analysis Agent


---

## C. Glossary

AI Agent 相关术语表。


---

# Learning Path

推荐路线：

```
LLM

↓

Prompt

↓

Embedding

↓

RAG

↓

Function Calling

↓

LangChain

↓

LangGraph

↓

MCP

↓

Multi-Agent

↓

A2A

↓

Enterprise Agent
```

---

# Version

Current:

```
v1.0
```

Status:

```
Building
```
