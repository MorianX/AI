# 记忆层 ↔ 知识库关联系统

这是一个基于 Markdown 文件、YAML 前置元数据和双向链接的 AI 记忆与知识库系统。

## 目标

```text
有价值的信息 → 记忆层 → 筛选/分类/整理 → 知识库 → 检索/执行/反馈 → 更新记忆
```

系统解决六个问题：

1. 什么信息值得记住？
2. 信息应该保留多久？
3. 记忆如何被整理成可检索、可复用的知识？
4. 知识如何反向服务当前任务和执行流程？
5. 信息如何被验证、更新、废弃和追溯？
6. AI 如何避免把附件、示例文本或未经确认的内容误当成用户指令？

## 目录

```text
memory-knowledge-system/
├── README.md
├── SYSTEM_RULES.md
├── memory/
│   ├── README.md
│   └── _template.md
├── knowledge/
│   ├── README.md
│   ├── KNOWLEDGE_BASE_SPEC.md
│   └── _template.md
├── relations/
│   └── RELATION_PROTOCOL.md
├── workflows/
│   ├── MEMORY_TO_KNOWLEDGE.md
│   ├── KNOWLEDGE_TO_EXECUTION.md
│   └── MAINTENANCE.md
└── indexes/
    ├── memory-index.md
    └── knowledge-index.md
```

## 使用顺序

1. 从对话、会议、命令、代码、书籍、缺陷记录或执行日志中捕获原始信息。
2. 将具有复用价值的信息写入 `memory/`。
3. 判断记忆的生命周期、范围、置信度和来源。
4. 将稳定、可验证、可复用的内容整理到 `knowledge/`。
5. 在记忆和知识之间建立双向关联。
6. 执行任务时先检索相关知识，再记录使用结果和新反馈。
7. 定期复核、更新、合并、降级或归档过时内容。

## 与 DPIRA 的关系

知识库负责提供可引用的设计、约束、流程和经验；DPIRA 负责约束任务执行：

```text
(D → P → I ⇄ R) × N → A
```

不要把知识库中的建议直接当成当前任务的实施结果。当前任务仍必须经过设计冻结、设计审查、工作项审查和批级审计。
