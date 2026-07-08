# BOOK_STRUCTURE.md

> AI-Agent-Interview-Handbook 全书结构设计规范（Book Structure Specification）

---

# 1. 文档目的（Purpose）

本文件定义 **AI-Agent-Interview-Handbook** 的整体组织结构、章节规划、知识递进关系及命名规范。

其目标是：

- 保持全书结构统一
- 保持知识递进清晰
- 保证章节粒度一致
- 方便长期维护与扩展
- 降低多人协作成本

本规范适用于整个仓库的所有文档。

---

# 2. 全书设计原则（Book Design Principles）

全书遵循以下设计原则：

- **系统化（Systematic）**：建立完整知识体系，而非零散知识点。
- **递进式（Progressive）**：遵循由浅入深、由原理到实践的学习路径。
- **工程化（Engineering）**：强调企业级架构与工程实践。
- **长期维护（Maintainable）**：支持持续更新，不因技术发展而整体失效。
- **面试导向（Interview-oriented）**：覆盖企业真实面试考点。

---

# 3. 知识体系（Knowledge Map）

全书建议按照以下学习顺序阅读：

```text
LLM Foundation
        │
        ▼
Prompt Engineering
        │
        ▼
Context Engineering
        │
        ▼
AI Agent Foundation
        │
        ▼
Planning
        │
        ▼
Memory
        │
        ▼
Workflow
        │
        ▼
Tool Calling
        │
        ▼
RAG
        │
        ▼
Multi-Agent
        │
        ▼
MCP
        │
        ▼
A2A
        │
        ▼
Production
        │
        ▼
Interview
```

章节之间存在明确的前置依赖关系，应尽量避免跳跃式组织。

---

# 4. 推荐目录结构（Repository Structure）

```text
docs/

├── 01-llm-foundation/
├── 02-prompt-engineering/
├── 03-context-engineering/
├── 04-agent-foundation/
├── 05-planning/
├── 06-memory/
├── 07-workflow/
├── 08-tool-calling/
├── 09-rag/
├── 10-multi-agent/
├── 11-agent-framework/
├── 12-mcp/
├── 13-a2a/
├── 14-production/
├── 15-interview/
└── appendix/
```

一级目录采用两位数字编号，按知识递进排序。

---

# 5. 一级目录职责（Top-level Modules）

| 目录 | 内容范围 |
|------|----------|
| 01-llm-foundation | LLM 基础知识、Transformer、Token、推理机制等 |
| 02-prompt-engineering | Prompt 设计原则、模式、优化方法 |
| 03-context-engineering | Context Window、上下文管理、上下文压缩 |
| 04-agent-foundation | Agent 基本概念、组成、生命周期 |
| 05-planning | Task Planning、Reasoning、Plan Execution |
| 06-memory | Short-term Memory、Long-term Memory、Memory 管理 |
| 07-workflow | Workflow、State Machine、Execution Flow |
| 08-tool-calling | Function Calling、Tool Calling、Tool Router |
| 09-rag | Retrieval、Embedding、Vector Database、Hybrid Search |
| 10-multi-agent | Multi-Agent 协作、通信、协调机制 |
| 11-agent-framework | LangGraph、AutoGen、CrewAI 等框架解析 |
| 12-mcp | Model Context Protocol 原理与实践 |
| 13-a2a | Agent2Agent 协议、跨 Agent 协作 |
| 14-production | 企业架构、部署、监控、安全、性能优化 |
| 15-interview | 面试知识总结、系统设计、经典题库 |
| appendix | 附录、术语表、学习路线、参考资料 |

---

# 6. 一级目录命名规范（Directory Naming）

统一采用：

```text
数字-英文名称
```

例如：

```text
01-llm-foundation

10-multi-agent

14-production
```

要求：

- 全部小写
- 使用 kebab-case
- 不使用空格
- 不使用中文
- 不使用下划线

禁止：

```text
LLMFoundation

LLM_Foundation

第一章

LLM基础
```

---

# 7. 文件命名规范（File Naming）

章节文件统一采用：

```text
01-overview.md

02-principle.md

03-architecture.md

04-components.md

05-workflow.md

06-code.md

07-enterprise.md

08-best-practice.md

09-common-mistakes.md

10-interview.md
```

要求：

- 两位数字编号
- 小写英文
- kebab-case
- 文件职责单一

禁止：

```text
new.md

temp.md

draft.md

test.md
```

---

# 8. 标准章节模板（Standard Chapter Template）

除概览章节外，每个技术主题建议采用以下结构：

```text
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

如无特殊原因，应保持章节顺序一致。

---

# 9. 内容粒度（Content Granularity）

一个文件只讨论一个核心主题。

推荐：

```text
Memory 分类

Memory 生命周期

Memory 压缩策略

Memory 持久化
```

不推荐：

```text
Memory 全部内容
```

建议单篇文档聚焦一个问题，保持阅读节奏。

---

# 10. 知识依赖关系（Knowledge Dependency）

每个章节建议在开头标明：

```text
前置知识

学习目标

阅读建议

预计阅读时间
```

结尾建议提供：

```text
本章总结

相关阅读

下一章节
```

帮助读者建立连续学习路径。

---

# 11. 内容复用原则（Content Reuse）

对于公共概念，应遵循：

- 首次详细讲解
- 后续章节引用
- 避免重复复制

例如：

- Token
- Embedding
- Context Window
- Attention
- Transformer

只在首次出现时进行系统说明。

---

# 12. 示例代码组织（Code Examples）

代码示例遵循渐进式设计：

第一层：

最小可运行示例

第二层：

模块级示例

第三层：

完整功能实现

第四层：

企业级实践

代码应服务于原理解释，而非追求复杂性。

---

# 13. 图示规范（Diagram Strategy）

优先使用可维护的文本图示。

推荐：

- Mermaid
- ASCII Diagram

避免：

- 截图
- 不可编辑图片
- 外部绘图工具导出的静态图片

所有图示应与正文同步维护。

---

# 14. 面试体系（Interview System）

每章保留对应的面试内容。

同时，在：

```text
docs/15-interview/
```

建立统一的面试知识库。

建议覆盖：

- 高频面试题
- 深度追问
- 系统设计题
- 开放性讨论题
- 企业真实案例分析

---

# 15. 附录设计（Appendix）

附录建议包括：

```text
术语表（Terminology）

英文缩写（Abbreviations）

经典论文（Papers）

优秀开源项目（Open Source）

学习路线（Learning Path）

推荐书籍（Books）

参考资料（References）
```

附录内容应独立维护，不与正文混合。

---

# 16. 扩展策略（Future Expansion）

未来新增章节时，应遵循编号递增原则。

例如：

```text
16-agent-security/

17-agent-evaluation/

18-agent-observability/

19-ai-safety/

20-case-study/
```

原则：

- 不修改已有编号
- 不打乱知识递进
- 保持命名一致

---

# 17. 长期维护规范（Maintenance Rules）

新增内容必须满足：

- 与现有目录保持一致
- 遵循统一章节模板
- 保持术语统一
- 保持代码风格一致
- 保持图示风格一致
- 保持知识递进关系

避免：

- 重复讲解
- 命名不一致
- 章节职责交叉
- 内容碎片化

---

# 18. 全书目标（Book Vision）

本书希望帮助读者逐步完成以下能力建设：

1. 理解 LLM 与 AI Agent 的核心原理。
2. 掌握 AI Agent 系统架构设计方法。
3. 熟悉主流 Agent Framework 的设计思想。
4. 能够独立开发企业级 AI Agent 应用。
5. 理解 Multi-Agent、MCP、A2A 等前沿技术。
6. 具备 AI Agent 岗位面试与系统设计能力。

最终形成一套兼具理论深度、工程实践与长期参考价值的 AI Agent 知识体系。

---

# Completion Status

**当前状态：** ✅ 已完成（Complete）

本文件已定义：

- 全书知识体系
- 目录组织方式
- 章节规划
- 命名规范
- 内容粒度
- 知识递进关系
- 长期扩展策略

后续一般无需频繁修改。

仅建议在以下情况更新本文件：

- 新增一级章节（例如新增 AI Safety、Agent Evaluation 等模块）
- 调整全书知识体系
- 调整目录组织结构
- 修订章节规划原则

普通章节内容更新无需修改本文件。

---

**下一步建议：**

建议继续编写：

> **TERMINOLOGY.md**

统一整个项目的术语规范，包括：

- 中英文术语映射
- 推荐用词
- 禁止混用的术语
- 缩写规范
- 大小写规范
- AI Agent 领域统一命名

该文件将作为整个项目的"术语字典"，所有后续文档均应遵循。
