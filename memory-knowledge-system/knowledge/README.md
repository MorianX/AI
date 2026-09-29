# 知识库

知识库存放经过筛选、结构化、验证并可以被 AI 检索和引用的内容。

本目录必须遵守 [KNOWLEDGE_BASE_SPEC.md](./KNOWLEDGE_BASE_SPEC.md)。

知识只按要解决的问题分类，使用以下 10 个主分类：

`concept`、`decisions`、`discussions`、`experiment`、`pitfalls`、`reference`、`rules`、`standards`、`sop`、`workflow`。

## 状态

- `draft`：已整理但尚未完成验证
- `reviewed`：已完成审查，可以在限定范围内引用
- `active`：当前有效的正式知识
- `deprecated`：已被新知识替代，不应作为默认依据
- `archived`：仅保留历史记录

## 知识质量要求

知识必须说明结论、适用条件、来源、验证方式、限制和更新时间。不能只保留脱离上下文的结论。

目录不是分类依据，不能通过建立多个类型子目录替代 `knowledge_type` 元数据。

使用 `_template.md` 创建新知识，并更新 `../indexes/knowledge-index.md`。
