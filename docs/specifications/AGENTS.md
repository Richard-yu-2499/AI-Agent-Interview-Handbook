# AGENTS.md

> AI Contributor Operating Specification  
> AI-Agent-Interview-Handbook AI 协作规范

---

# 1. Purpose

本文件定义 **AI-Agent-Interview-Handbook** 仓库中所有 AI Contributor（包括 ChatGPT、Claude、Gemini、Copilot、Cursor、Codeium 等）的统一协作规范。

目标：

- 保持整个项目风格一致
- 保证技术内容准确
- 保证长期可维护
- 避免 AI 生成内容质量波动
- 降低多人协作成本

任何 AI 在生成、修改、补充本仓库内容时，都应遵循本规范。

---

# 2. Project Position

本项目定位为：

> 一本长期维护、工程导向、出版社级质量的 AI Agent 开源电子书。

不是：

- Prompt 收集仓库
- Demo 示例仓库
- API 文档
- AI 新闻整理
- 博客合集

所有内容均应围绕：

> 原理 → 架构 → 工程 → 企业实践 → 面试

展开。

---

# 3. Writing Language

所有正文统一使用中文。

以下专业术语保留英文：

- LLM
- Agent
- AI Agent
- Workflow
- Memory
- Planning
- Tool Calling
- Function Calling
- MCP
- A2A
- RAG
- Prompt Engineering
- Context Engineering
- Multi-Agent
- Embedding
- Token
- Inference
- Fine-tuning
- Alignment

禁止为了中文化而创造新的术语。

---

# 4. Target Readers

默认读者具备：

- 基础编程能力
- 至少掌握一种后端语言
- 对 LLM 有基本了解

默认不解释：

- HTTP
- JSON
- REST
- Docker
- Git
- Python 基础语法

避免把内容写成零基础教程。

---

# 5. Writing Principles

所有内容遵循以下原则。

## 5.1 Explain Why First

优先回答：

为什么会出现？

然后再介绍：

- 是什么
- 如何实现
- 如何使用

不要直接进入 API 或代码示例。

---

## 5.2 Principle Before Practice

优先讲清楚：

- 核心思想
- 工作原理
- 设计目标

之后再介绍：

- API
- Framework
- SDK

---

## 5.3 Architecture Before Code

先说明：

系统架构

再说明：

模块组成

最后再写代码。

不要先写代码再解释原理。

---

## 5.4 Engineering Before Demo

所有内容优先采用企业级实践。

避免：

"Hello World"

式示例占据大量篇幅。

---

## 5.5 Long-term Maintainability

所有内容必须具有长期阅读价值。

避免：

- 新闻风格
- 时效性标题
- 热点追踪
- 情绪化表达

---

# 6. Standard Chapter Structure

除特殊章节外，所有技术章节统一采用以下结构。

```
为什么出现

核心原理

整体架构

关键组件

工作流程

代码示例

企业实践

最佳实践

常见误区

面试题

参考资料
```

章节顺序保持一致。

---

# 7. Explanation Style

解释概念时建议采用以下顺序。

第一步：

问题背景

第二步：

为什么会出现

第三步：

核心思想

第四步：

工作流程

第五步：

工程实现

第六步：

优缺点分析

第七步：

企业实践

避免直接给定义。

---

# 8. Code Style

代码仅用于解释核心思想。

要求：

- 尽量完整
- 可以运行
- 变量命名清晰
- 注释必要即可
- 不堆砌无意义代码

优先语言：

- Python
- TypeScript

必要时补充：

- Java
- Go

---

# 9. Architecture Description

涉及系统设计时，应尽量说明：

模块职责

数据流

生命周期

上下游关系

依赖关系

扩展方式

性能瓶颈

避免只介绍单个类或函数。

---

# 10. Enterprise Practice

企业实践部分至少回答以下问题。

为什么这样设计？

有哪些替代方案？

为什么没有采用其他方案？

系统瓶颈在哪里？

如何扩展？

如何监控？

如何保证稳定性？

如何保证可维护性？

---

# 11. Interview Section

每章必须包含面试部分。

建议包括：

## 高频问题

适合一面。

---

## 深度追问

适合二面。

---

## 系统设计题

适合高级岗位。

---

## 开放问题

帮助读者建立系统思考能力。

---

每道题建议包含：

问题

考察点

参考答案

延伸问题

---

# 12. Diagram Guidelines

建议尽量使用 Markdown 可维护格式。

优先：

```
ASCII Diagram
```

或者：

```
Mermaid
```

避免：

截图

图片

不可编辑流程图

---

# 13. Markdown Style

统一采用：

```
#

##

###

```

不要超过三级标题。

列表统一使用：

```
-

1.
```

代码块注明语言。

例如：

```python
```

```typescript
```

---

# 14. Tone

保持：

专业

客观

严谨

中立

避免：

聊天风格

营销语言

夸张表达

AI 自我描述

例如避免：

> 我认为……

> 我觉得……

> 非常神奇……

---

# 15. Content Quality Requirements

内容应达到：

出版社技术图书质量。

要求：

逻辑完整

术语统一

结构一致

可长期维护

可持续扩展

避免重复解释同一概念。

---

# 16. What AI Should Avoid

禁止生成以下内容。

## 不完整解释

例如：

只介绍概念。

没有说明为什么。

---

## API 堆砌

不要把官方文档复制成教程。

---

## Demo 驱动

不要只围绕 Demo 展开。

---

## 大量重复

不要反复解释：

LLM

Prompt

Token

Context

除非章节确实需要。

---

## 无来源结论

涉及：

性能

Benchmark

论文结论

行业数据

应注明来源。

---

## 模糊描述

避免：

"一般来说"

"很多时候"

"通常"

应尽量给出明确条件。

---

# 17. Consistency Rules

新增内容必须保持：

术语一致

标题一致

代码风格一致

图示风格一致

章节顺序一致

命名方式一致

不要混用不同表达。

例如统一使用：

Tool Calling

不要交替写：

Tool Call

Tool Invocation

Function Tool

---

# 18. Commit Requirements

所有 AI 输出必须满足：

- 可以直接 Commit
- Markdown 无格式错误
- 不包含聊天内容
- 不包含解释性文字
- 不包含 AI 回复痕迹
- 不包含"以下是生成内容"等前缀
- 不包含 Emoji（除非文档明确需要）

---

# 19. Output Rules

默认情况下：

一个回复仅生成一个文件。

不要同时生成多个文件。

如果内容较长，应保证：

一个文件

一次复制

直接 Commit

---

# 20. Repository Philosophy

本项目追求的不是：

**内容最多。**

而是：

**内容最准确。**

不是：

**更新最快。**

而是：

**生命周期最长。**

不是：

**Demo 最丰富。**

而是：

**工程价值最高。**

最终目标：

打造一套可以持续维护、多年仍具参考价值的 AI Agent 工程知识体系，并成为 AI Agent 学习与面试领域的高质量开源电子书。
