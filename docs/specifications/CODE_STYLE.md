# CODE_STYLE.md

> 本文档定义《AI-Agent-Interview-Handbook》项目中所有代码示例、配置示例、API
> 示例、Prompt 示例以及 Agent 系统示例的统一编写规范。
>
> 目标是保证 Handbook 具备长期维护能力，并达到技术出版社级内容质量。

------------------------------------------------------------------------

# 1. 文档目标

CODE_STYLE.md 用于规范：

-   代码展示方式
-   示例代码结构
-   配置文件格式
-   API 示例格式
-   Agent Workflow 示例
-   Multi-Agent 示例
-   Prompt 示例
-   Pseudocode 表达方式

核心目标：

-   Readability
-   Consistency
-   Maintainability
-   Reproducibility
-   Interview Friendliness

所有示例必须服务于：

> 解释技术思想，而不是展示无关代码数量。

------------------------------------------------------------------------

# 2. 基本原则

## 2.1 Concept First

代码应该优先表达：

-   架构思想
-   核心流程
-   关键算法
-   设计模式
-   工程实践

避免：

-   大量初始化代码
-   无关业务逻辑
-   复杂依赖配置

------------------------------------------------------------------------

## 2.2 Minimal Complete Example

示例应该：

-   足够完整
-   容易理解
-   可以扩展
-   可以验证

推荐：

``` python
planner = Planner()

plan = planner.create_plan(task)

executor.execute(plan)
```

避免展示无法理解的大型工程代码。

------------------------------------------------------------------------

## 2.3 Runnable First

如果示例标记为：

-   Example
-   Demo
-   Tutorial

需要尽量保证：

-   输入明确
-   输出明确
-   依赖明确

如果是伪代码，需要明确：

``` text
This example is simplified pseudocode.
```

------------------------------------------------------------------------

# 3. Markdown Code Block 规范

所有代码块必须声明语言。

正确：

``` python
print("Hello Agent")
```

错误：

    print("Hello Agent")

------------------------------------------------------------------------

## 3.1 标准语言

  类型         Markdown 标识
  ------------ ---------------
  Python       python
  JavaScript   javascript
  TypeScript   typescript
  Go           go
  Java         java
  Rust         rust
  Shell        bash
  JSON         json
  YAML         yaml
  HTTP         http
  SQL          sql
  Prompt       text

------------------------------------------------------------------------

# 4. 通用代码规范

## 4.1 命名规则

  类型       规范
  ---------- ------------------------
  Variable   snake_case / camelCase
  Function   snake_case / camelCase
  Class      PascalCase
  Constant   UPPER_CASE

------------------------------------------------------------------------

## 4.2 注释规范

注释应该解释：

-   为什么这样设计
-   为什么采用该方案
-   存在哪些限制

推荐：

``` python
# Planner only generates execution plans.
# Executor performs actual actions.
```

避免：

``` python
# Create planner
planner = Planner()
```

------------------------------------------------------------------------

## 4.3 长代码限制

单个代码示例：

推荐：

-   小于 60 行
-   单一主题
-   无无关逻辑

超过限制：

应该：

-   拆分
-   提取核心逻辑
-   添加省略说明

------------------------------------------------------------------------

# 5. Python 规范

遵循：

-   PEP 8
-   Type Hint
-   Clear Naming

## 5.1 类型标注

推荐：

``` python
def execute(task: str) -> str:
    return result
```

------------------------------------------------------------------------

## 5.2 Import 顺序

顺序：

1.  Standard Library
2.  Third-party Library
3.  Internal Module

示例：

``` python
import json

from openai import OpenAI

from agent.memory import Memory
```

------------------------------------------------------------------------

## 5.3 Agent Python 示例

推荐体现：

``` python
class Agent:

    def plan(self):
        pass

    def execute(self):
        pass

    def reflect(self):
        pass
```

------------------------------------------------------------------------

# 6. TypeScript / JavaScript 规范

## 6.1 变量

推荐：

``` typescript
const agent = new Agent();
```

避免：

``` javascript
var agent = new Agent();
```

------------------------------------------------------------------------

## 6.2 命名

使用：

-   camelCase
-   PascalCase

示例：

``` typescript
class AgentExecutor {}

const memoryManager = {};
```

------------------------------------------------------------------------

# 7. Go / Java / Rust 规范

## Go

遵循：

-   gofmt
-   官方命名方式

## Java

要求：

-   Class 使用 PascalCase
-   Method 使用 camelCase
-   一个 public class 一个文件

## Rust

遵循：

-   Rustfmt
-   官方命名规范

------------------------------------------------------------------------

# 8. Configuration 规范

## 8.1 JSON

要求：

-   双引号
-   两个空格缩进

示例：

``` json
{
  "model": "YOUR_MODEL"
}
```

------------------------------------------------------------------------

## 8.2 YAML

要求：

-   两个空格缩进
-   禁止 Tab

示例：

``` yaml
agent:
  name: planner
  enabled: true
```

------------------------------------------------------------------------

# 9. Secret 与环境变量规范

禁止：

-   API Key
-   Token
-   Password
-   Private URL

错误：

``` text
sk-xxxxxxxx
```

正确：

``` bash
OPENAI_API_KEY=YOUR_API_KEY
```

统一 Placeholder：

-   YOUR_API_KEY
-   YOUR_MODEL
-   YOUR_ENDPOINT
-   YOUR_TOKEN

------------------------------------------------------------------------

# 10. Prompt 示例规范

Prompt 使用：

``` text
You are an AI Agent.

Your task is to solve the problem.
```

必须明确：

-   Role
-   Goal
-   Constraint
-   Expected Output

------------------------------------------------------------------------

# 11. API 示例规范

API 示例顺序：

1.  Method
2.  Endpoint
3.  Headers
4.  Request
5.  Response

示例：

``` http
POST /v1/agents/run HTTP/1.1
Authorization: Bearer YOUR_TOKEN
```

------------------------------------------------------------------------

# 12. AI Agent 示例规范

所有 Agent 示例应该尽量体现：

-   Agent
-   Planning
-   Execution
-   Tool Calling
-   Memory
-   Reflection

推荐：

``` text
User Task

↓

Planner

↓

Executor

↓

Tool

↓

Memory

↓

Final Answer
```

------------------------------------------------------------------------

# 13. Tool Calling 示例规范

Tool 示例需要说明：

-   Tool Name
-   Input Schema
-   Output Schema
-   Error Handling

例如：

``` json
{
  "name": "search",
  "parameters": {
    "query": "string"
  }
}
```

------------------------------------------------------------------------

# 14. MCP / A2A / Multi-Agent 规范

涉及：

-   MCP
-   A2A
-   Multi-Agent System

必须说明：

-   Agent Role
-   Communication Flow
-   Message Schema
-   Capability Boundary

避免：

只展示 API 调用而不解释系统关系。

------------------------------------------------------------------------

# 15. Production Code 示例规范

生产级示例应考虑：

-   Error Handling
-   Logging
-   Observability
-   Security
-   Testing

不要展示：

没有错误处理的假生产代码。

------------------------------------------------------------------------

# 16. Interview 示例规范

面试场景代码：

应该：

-   突出核心思想
-   控制复杂度
-   易于白板表达

避免：

展示完整生产系统。

------------------------------------------------------------------------

# 17. 错误示例规范

错误代码必须明确：

``` text
❌ Incorrect Example
```

推荐代码必须明确：

``` text
✅ Recommended Example
```

------------------------------------------------------------------------

# 18. Review Checklist

代码提交前检查：

-   是否服务章节主题
-   是否容易理解
-   是否包含真实 Secret
-   是否可以复制
-   是否符合命名规范
-   是否存在隐藏依赖
-   是否容易维护

------------------------------------------------------------------------

# 19. 与其它规范关系

  文件                   职责
  ---------------------- --------------
  STYLE_GUIDE.md         全局写作风格
  WRITING_GUIDE.md       内容生产流程
  TERMINOLOGY.md         专业术语统一
  DIAGRAM_GUIDE.md       图示规范
  QUALITY_CHECKLIST.md   质量审核

------------------------------------------------------------------------

# Completion Status

## 当前状态

✅ CODE_STYLE.md Final Version 已完成。

该文件可以直接提交到：

`handbook_v1.0`

分支。

## 什么时候需要更新

以下情况需要更新：

-   新增编程语言
-   新增 Agent Framework
-   新增协议示例规范
-   项目进入新版本

## 下一步建议

继续生成：

`QUALITY_CHECKLIST.md`
