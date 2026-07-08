# DIAGRAM_GUIDE.md

> AI-Agent-Interview-Handbook 图示规范（Diagram Guide）

---

# 1. 文档目的（Purpose）

本文档定义 **AI-Agent-Interview-Handbook** 全书统一的图示规范。

目标：

- 保持所有图示风格一致
- 保证图示可维护、可版本管理
- 保证 GitHub 原生可渲染
- 降低后期维护成本
- 提高阅读体验

所有章节涉及系统架构、流程、状态变化、模块关系时，应优先使用本文档规定的图示方式。

---

# 2. 基本原则（General Principles）

所有图示应遵循以下原则：

- 简洁优先（Simple）
- 可维护（Maintainable）
- 可版本管理（Version Controlled）
- 与正文同步更新
- 服务于理解，而非装饰

图示应帮助读者理解架构和流程，而不是增加阅读负担。

---

# 3. 推荐图示类型（Diagram Types）

推荐使用以下图示：

| 图示类型 | 推荐程度 | 使用场景 |
|----------|----------|----------|
| Mermaid Flowchart | ⭐⭐⭐⭐⭐ | 系统流程 |
| Mermaid Sequence Diagram | ⭐⭐⭐⭐⭐ | 时序分析 |
| Mermaid Class Diagram | ⭐⭐⭐⭐ | 模块关系 |
| Mermaid State Diagram | ⭐⭐⭐⭐ | 生命周期 |
| Mermaid Mindmap | ⭐⭐⭐ | 知识结构 |
| ASCII Diagram | ⭐⭐⭐⭐ | 简单架构说明 |

原则：

优先 Mermaid。

简单结构可使用 ASCII。

---

# 4. 禁止使用（Not Recommended）

不建议：

- 截图
- PPT 导出的图片
- Visio 静态图片
- Draw.io 导出的 PNG
- 无法编辑的流程图

原因：

- 无法进行 Git Diff
- 无法代码审查
- 难以长期维护

---

# 5. Flowchart 规范

适用于：

- 工作流程
- 数据流
- 请求处理流程
- Agent 执行流程

建议：

- 自上而下（TD）
- 保持节点数量适中
- 节点名称简洁

推荐：

```mermaid
flowchart TD

A[User]

↓

B[Agent]

↓

C[LLM]

↓

D[Tool]

↓

E[Result]
```

---

# 6. Sequence Diagram 规范

适用于：

- Tool Calling
- MCP
- A2A
- Multi-Agent
- API 调用

推荐：

```mermaid
sequenceDiagram

User->>Agent

Agent->>LLM

LLM-->>Agent

Agent->>Tool

Tool-->>Agent

Agent-->>User
```

突出交互顺序。

---

# 7. State Diagram 规范

适用于：

- 生命周期
- 状态机
- Workflow
- Task Execution

推荐展示：

状态

事件

状态转换

避免复杂条件判断。

---

# 8. Class Diagram 规范

适用于：

- Framework 架构
- SDK
- 模块关系

关注：

职责

依赖关系

组合关系

避免展示实现细节。

---

# 9. Architecture Diagram

架构图建议采用分层设计：

```text
Application Layer

↓

Agent Layer

↓

Workflow Layer

↓

Tool Layer

↓

LLM Layer

↓

Infrastructure
```

每层职责明确。

不要画成交叉网状结构。

---

# 10. ASCII Diagram

适用于：

- 小型架构
- 文本说明
- GitHub 阅读

例如：

```text
+---------+

User

+---------+

|

v

+---------+

Agent

+---------+

|

v

+---------+

LLM

+---------+
```

保证字体对齐。

---

# 11. 图示命名规范

正文引用统一采用：

图 1-1

图 2-3

图 5-2

编号建议：

章节号-序号

例如：

图 4-1

图 4-2

图 4-3

---

# 12. 图示说明

每张图建议包含：

图标题

一句话说明

正文解释

例如：

> 图 6-2 Agent Planning 执行流程

随后解释：

输入

处理

输出

不要只放图不解释。

---

# 13. 图示复杂度控制

建议：

一个图只表达一个主题。

推荐：

- 一个流程
- 一个架构
- 一个生命周期

避免：

多个系统

多个流程

多个模块

全部画在一张图中。

---

# 14. 与正文关系

正文负责：

解释

分析

总结

图示负责：

展示关系

展示流程

展示结构

不要让图替代正文。

---

# 15. 长期维护建议

修改正文时，应同步检查：

- 图示是否一致
- 节点名称是否一致
- 模块名称是否一致
- 顺序是否一致

保证图文一致。

---

# Completion Status

**当前状态：** ✅ 已完成（Complete）

本文件定义了全书统一图示规范，包括 Mermaid、ASCII Diagram、架构图、流程图及图文对应关系。

后续仅在以下情况更新：

- GitHub Markdown 支持新的图示能力
- 项目新增统一图示类型
- 调整全书图示规范

普通章节无需修改本文件。
