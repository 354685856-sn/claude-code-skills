---
name: env-setup
description: 环境设置与配置 - 自动化开发环境配置
version: 1.0.0
---

# Environment Setup Skill

## 用途
自动化开发环境配置、依赖管理和工具版本管理。

## 功能范围

### 1. 开发环境
- Node.js/Python/Go 版本
- 包管理器配置
- IDE 设置

### 2. 依赖管理
- 安装项目依赖
- 检查版本兼容性
- 更新过时的依赖

### 3. 工具配置
- Git hooks 设置
- Linter/Formatter 配置
- 数据库迁移

### 4. 环境变量
- .env 文件生成
- 密钥配置
- 服务连接配置

## 使用方法

```bash
/claude "使用 env-setup skill 设置开发环境"
/claude "使用 env-setup skill 检查依赖"
```

## 输出格式

```markdown
## 环境配置报告

### 当前状态
- Node.js: vXX.X.X
- 依赖状态：正常/需要更新

### 已完成配置
- 列表...

### 需要手动配置
- 列表及说明
```
