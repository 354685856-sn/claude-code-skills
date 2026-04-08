---
name: prompt-cache-optimize
description: Prompt Caching 优化 - 根据 Thariq 的 7 条经验优化提示词结构
version: 1.0.0
---

# Prompt Cache Optimization Skill

## 用途
根据 Thariq Shihipar (Claude Code 团队) 的 7 条经验优化提示词缓存命中率。

## Thariq 的 7 条经验

1. **前缀匹配** - 稳定内容放开头，可变内容放末尾
2. **子代理继承** - 字节级复制父上下文
3. **模型变更破坏缓存** - 保持系统提示词稳定
4. **消息顺序** - 严格追加，避免重排序
5. **system/messages 分离** - 不变指令放 system
6. **工具定义放末尾** - 减少前缀缓存破坏
7. **核心基础设施** - 缓存命中率下降=SEV

## 优化检查清单

### 提示词结构
- [ ] 系统指令是否在 `system` 字段
- [ ] 工具定义是否在消息末尾
- [ ] 用户输入是否在最后
- [ ] 历史消息是否按顺序追加

### 缓存监控
- [ ] 是否记录缓存命中率
- [ ] 是否设置告警阈值
- [ ] 是否分析缓存破坏原因

## 使用方法

```bash
/claude "使用 prompt-cache-optimize skill 优化这个提示词"
```

## 输出格式

```markdown
## Prompt Cache 优化报告

### 当前命中率
- 估计命中率：X%

### 优化建议
1. 将 [内容] 移到 system 字段
2. 将 [工具定义] 移到末尾
3. 保持消息追加顺序

### 预期改进
- 命中率提升到：Y%
- 成本降低：Z%
```
