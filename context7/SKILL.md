---
name: context7
description: 查找并理解最新的技术文档和 API 参考
user-invocable: true
context: fork
agent: claude-code-guide
allowed-tools: WebFetch, WebSearch, Read, Grep
---

# Context7 - 最新文档查找技能

你的任务是查找并理解最新的技术文档，确保代码实现基于最新的 API 和最佳实践。

## 工作流程

### 1. 确定需求
- 理解用户需要查找的技术/库/API
- 确定关键问题和使用场景

### 2. 搜索文档
- 优先查找官方文档
- 查找最新的 GitHub README
- 搜索相关的技术博客和教程

### 3. 整理信息
- 提取关键的 API 用法
- 记录版本差异和废弃内容
- 总结最佳实践

### 4. 输出报告
按以下格式输出：

```
## 核心概念
[简要说明]

## API 用法
[代码示例]

## 注意事项
[版本要求、废弃内容等]

## 参考链接
[文档 URL]
```

## 适用场景

- 集成新的第三方库
- 查询 API 最新用法
- 理解技术实现细节
- 对比不同方案的优劣
