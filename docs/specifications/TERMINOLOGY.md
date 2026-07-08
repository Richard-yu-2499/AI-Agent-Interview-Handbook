# TERMINOLOGY.md

> AI-Agent-Interview-Handbook 术语规范（Terminology Specification）

---

# 1. 文档目的（Purpose）

本文档定义 **AI-Agent-Interview-Handbook** 全书统一使用的专业术语、英文缩写、命名规则及中英文对应关系。

目标：

- 保持全书术语一致
- 避免同一概念出现多个名称
- 降低读者理解成本
- 保证长期维护的一致性
- 为所有 AI Contributor 提供统一术语规范

除引用论文、官方文档或历史名称外，本项目所有内容均应遵循本规范。

---

# 2. 基本原则（General Principles）

## 中文为主

正文统一使用中文。

例如：

> AI Agent 的核心能力包括 Planning、Memory 与 Tool Calling。

而不是：

> The AI Agent uses Planning to...

---

## 保留英文专业术语

对于行业已经广泛接受的专业术语，保留英文，不强制翻译。

例如：

- LLM
- Agent
- Prompt
- Workflow
- Memory
- Planning
- Tool Calling
- Function Calling
- Embedding
- Token
- Context Window

---

## 首次出现规则

第一次出现时采用：

```
中文（English）
```

例如：

```
上下文工程（Context Engineering）
```

后续统一使用：

```
Context Engineering
```

或：

```
上下文工程
```

避免反复中英文混排。

---

# 3. 核心术语规范（Core Terminology）

| 推荐术语 | 不推荐 |
|----------|--------|
| AI Agent | Agent System、智能代理系统 |
| LLM | 大语言模型（首次可说明） |
| Prompt | 提示词 |
| Prompt Engineering | Prompt 工程 |
| Context Engineering | Context 工程 |
| Workflow | 工作流（首次可说明） |
| Planning | Planning（不建议翻译为"规划器"） |
| Memory | Memory（不建议统一翻译为"记忆模块"） |
| Tool Calling | Tool Call、工具调用接口 |
| Function Calling | Function Call |
| Multi-Agent | Multi Agent、MultiAgent |
| RAG | Retrieval-Augmented Generation 全称首次说明 |
| MCP | Model Context Protocol 全称首次说明 |
| A2A | Agent2Agent 全称首次说明 |

---

# 4. 大小写规范（Capitalization）

统一采用官方大小写。

| 正确 | 错误 |
|------|------|
| AI Agent | Ai Agent |
| LLM | Llm |
| GPT-4 | Gpt4 |
| MCP | mcp |
| A2A | a2a |
| LangGraph | langgraph |
| CrewAI | CrewAi |
| AutoGen | Autogen |

禁止随意修改官方名称。

---

# 5. 缩写规范（Abbreviations）

首次出现建议写法：

```
Large Language Model（LLM）
```

之后统一使用：

```
LLM
```

同样适用于：

- RAG
- MCP
- A2A
- API
- SDK
- RPC

---

# 6. Framework 命名

统一采用官方名称。

例如：

- LangGraph
- AutoGen
- CrewAI
- Semantic Kernel
- OpenAI Agents SDK

禁止自行修改名称或缩写。

---

# 7. 技术术语统一

以下术语保持固定表达：

| 推荐 | 不推荐 |
|------|--------|
| Context Window | 上下文长度、窗口大小（混用） |
| Embedding | 向量化 |
| Vector Database | 向量数据库 |
| Retrieval | 检索 |
| Inference | 推理 |
| Fine-tuning | 微调 |
| Alignment | 对齐 |
| Hallucination | 幻觉 |
| Reasoning | 推理能力（根据上下文说明） |

---

# 8. 命名风格（Naming Style）

文档标题：

- 中文

目录名称：

- 英文
- kebab-case

代码：

- 遵循对应语言官方规范

Mermaid：

- 使用英文节点名称
- 注释使用中文

---

# 9. 企业名称

企业名称保持官方写法。

例如：

- OpenAI
- Anthropic
- Google DeepMind
- Microsoft
- Meta

禁止自行翻译企业名称。

---

# 10. 论文引用

论文名称保持英文原文。

例如：

- Attention Is All You Need
- ReAct
- Toolformer
- Tree of Thoughts

正文可增加中文解释，但标题不翻译。

---

# 11. 常见混用示例

| 推荐 | 不推荐 |
|------|--------|
| Multi-Agent | Multi Agent |
| Tool Calling | Tool Call |
| AI Agent | AI智能体（全文混用） |
| Context Engineering | Context 管理 |
| Function Calling | Function Call |

---

# 12. 新术语引入原则

新增术语应满足：

1. 来源于官方文档、论文或行业共识。
2. 首次出现提供必要说明。
3. 与已有术语保持一致。
4. 不随意创造新名词。

若存在多个译法，应优先采用行业主流表达。

---

# Completion Status

**当前状态：** ✅ 已完成（Complete）

本文件定义了全书统一术语、命名规则及缩写规范。

后续仅在以下情况更新：

- 新增重要 AI Agent 领域术语
- 官方命名发生变化
- 行业形成新的统一表达

普通章节无需修改本文件。

---

# 下一步建议

建议继续编写：

> **WRITING_GUIDE.md**

进一步规范章节组织、段落结构、示例写法、图示引用及引用格式，为后续所有正文提供统一写作标准。
