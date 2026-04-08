---
name: doc-gen
description: 文档生成与更新 - 自动生成 API 文档并保持与代码同步
version: 1.0.0
---

# Documentation Generation Skill

## 用途
自动生成或更新 API 文档、README、代码注释等。

## 文档类型

### 1. API 文档
- OpenAPI/Swagger 规范
- GraphQL Schema 文档
- RESTful API 参考

### 2. 代码文档
- JSDoc/TypeDoc 注释
- Python docstrings
- Go doc comments

### 3. 项目文档
- README.md
- CONTRIBUTING.md
- CHANGELOG.md
- 架构文档

## 使用方法

```bash
/claude "使用 doc-gen skill 生成这个模块的 API 文档"
/claude "使用 doc-gen skill 更新 README"
```

## 文档生成原则

1. **准确性** - 文档必须与代码一致
2. **完整性** - 覆盖所有公开 API
3. **示例驱动** - 包含使用示例
4. **可搜索** - 结构清晰便于查找

## 输出格式

```markdown
## 文档更新报告

### 生成的文档
- 文件列表

### 更新的文档
- 文件列表及变更

### 需要同步的问题
- 发现的问题列表
```
