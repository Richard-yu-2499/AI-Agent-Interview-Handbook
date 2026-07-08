# REFERENCES_GUIDE.md

> 本文档定义《AI-Agent-Interview-Handbook》项目中技术资料、论文、官方文档、代码仓库以及外部资源的引用规范。
>
> 目标是保证 Handbook 中所有引用内容具备可靠性、可追溯性和长期维护价值。

------------------------------------------------------------------------

# 1. 文档目标

REFERENCES_GUIDE.md 用于规范：

-   Research Paper 引用
-   Official Documentation 引用
-   Technical Report 引用
-   GitHub Repository 引用
-   Standard Specification 引用
-   External Resource 引用

核心目标：

> 让读者能够追溯知识来源，并进一步深入学习。

------------------------------------------------------------------------

# 2. 引用基本原则

## 2.1 优先官方来源

引用优先级：

1.  Official Documentation
2.  Original Paper
3.  Official Technical Report
4.  Maintained Open Source Repository
5.  高质量技术文章

避免：

-   无来源内容
-   内容农场
-   未验证博客
-   二次转载

------------------------------------------------------------------------

## 2.2 引用必须服务于内容

引用应该支持：

-   技术事实
-   历史背景
-   设计来源
-   API 行为
-   标准定义

避免：

为了增加引用数量而引用。

------------------------------------------------------------------------

# 3. 引用类型规范

## 3.1 Research Paper

适用于：

-   新模型架构
-   Agent 方法
-   Algorithm
-   Benchmark
-   理论研究

推荐格式：

``` text
Author(s).
Paper Title.
Conference / Journal.
Year.
URL / DOI.
```

示例：

``` text
Yao et al.
ReAct: Synergizing Reasoning and Acting in Language Models.
2023.
```

------------------------------------------------------------------------

## 3.2 Official Documentation

适用于：

-   API
-   SDK
-   Framework
-   Protocol

包含：

-   产品名称
-   文档名称
-   访问地址
-   更新时间（如需要）

示例：

``` text
OpenAI API Documentation.
Official Documentation.
```

------------------------------------------------------------------------

## 3.3 GitHub Repository

引用开源项目时：

需要说明：

-   项目名称
-   Organization / Author
-   用途
-   访问地址

示例：

``` text
Project:
LangGraph

Purpose:
Graph-based Agent Workflow Framework.
```

------------------------------------------------------------------------

## 3.4 Standard Specification

涉及：

-   Protocol
-   Interface
-   Communication Standard

必须引用：

-   标准名称
-   发布组织
-   版本

例如：

``` text
Model Context Protocol Specification.
Version information.
```

------------------------------------------------------------------------

# 4. AI Agent 专项引用规范

## 4.1 Agent Architecture

涉及：

-   Planning
-   Reasoning
-   Tool Use
-   Memory
-   Reflection

应优先引用：

-   Original Paper
-   Framework Documentation

------------------------------------------------------------------------

## 4.2 Multi-Agent System

涉及：

-   Agent Collaboration
-   Communication
-   Coordination
-   Negotiation

引用应覆盖：

-   理论来源
-   实现框架
-   工程实践

------------------------------------------------------------------------

## 4.3 MCP / A2A

涉及协议时：

必须引用：

-   官方 Specification
-   官方 Repository
-   Version 信息

避免只引用博客解释。

------------------------------------------------------------------------

# 5. 文中引用规范

## 5.1 首次出现

首次介绍技术时：

应该提供来源。

例如：

``` text
ReAct (Reasoning and Acting) was introduced in ...
```

------------------------------------------------------------------------

## 5.2 后续引用

同一章节：

无需重复完整引用。

保持：

-   简洁
-   清晰

------------------------------------------------------------------------

# 6. References Section 规范

每章如果包含引用：

建议增加：

``` markdown
## References
```

结构：

``` text
[1] Paper / Documentation Name

[2] Paper / Documentation Name
```

------------------------------------------------------------------------

# 7. 时间敏感内容

以下内容需要关注时间：

-   Model Capability
-   API Feature
-   Framework Version
-   Pricing
-   Product Availability

引用时建议注明：

``` text
Updated: YYYY-MM
```

------------------------------------------------------------------------

# 8. 引用质量检查

提交前确认：

-   来源真实存在
-   链接有效
-   作者正确
-   时间正确
-   内容相关

------------------------------------------------------------------------

# 9. 不推荐引用

避免：

-   无作者博客
-   自动生成文章
-   无验证论坛内容
-   搜索摘要
-   社交媒体碎片信息

------------------------------------------------------------------------

# 10. 版本维护

对于快速变化领域：

例如：

-   LLM
-   Agent Framework
-   API Platform

需要记录：

-   Version
-   Release Date
-   Compatibility

------------------------------------------------------------------------

# 11. 与其它规范关系

  文件                   职责
  ---------------------- --------------
  STYLE_GUIDE.md         全局写作风格
  WRITING_GUIDE.md       内容生产流程
  CODE_STYLE.md          代码规范
  QUALITY_CHECKLIST.md   质量审核
  TERMINOLOGY.md         术语规范
  DIAGRAM_GUIDE.md       图示规范

------------------------------------------------------------------------

# Completion Status

## 当前状态

✅ REFERENCES_GUIDE.md 已完成。

该文件可以直接提交到：

`handbook_v1.0`

分支。

## 什么时候需要更新

以下情况需要更新：

-   新增引用类型
-   新增出版规范
-   新增 AI Agent 领域标准
-   引用流程变化

## 下一步建议

规范文件阶段完成。

下一阶段可以进入：

-   Chapter 内容开发
-   Interview Question 编写
-   Architecture Deep Dive 编写
