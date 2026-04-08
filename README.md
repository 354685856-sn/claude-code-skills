# 楠哥的 Claude Code Skills

**作者**: 354685856-sn (楠哥)

基于 Thariq Shihipar (Claude Code 团队成员) 的 "Lessons from Building Claude Code: How We Use Skills" 文章创建的 Skills 集合。

## Skills 列表 (按 Thariq 9 大类型分类)

| Skill | 类型 | 用途 |
|-------|------|------|
| [context7](./context7/) | 1. 库与 API 参考 | 查找最新技术文档和 API 参考 |
| [product-verify](./product-verify/) | 2. 产品验证 | 验证代码更改是否符合产品需求 |
| [data-fetch](./data-fetch/) | 3. 数据获取与分析 | 获取日志、指标、用户反馈 |
| [gsd](./gsd/) | 4. 业务流程与自动化 | 三阶段任务执行框架 |
| [code-review](./code-review/) | 5. 代码审查与质量检查 | 检查代码质量和潜在问题 |
| [test-gen](./test-gen/) | 6. 测试生成与执行 | 生成针对性测试并执行 |
| [doc-gen](./doc-gen/) | 7. 文档生成与更新 | 自动生成 API 文档 |
| [security-check](./security-check/) | 8. 安全与合规检查 | 检查代码安全规范 |
| [env-setup](./env-setup/) | 9. 环境设置与配置 | 自动化开发环境配置 |

## 额外 Skills

| Skill | 用途 |
|-------|------|
| [superpowers](./superpowers/) | 增强型开发助手 |
| [prompt-cache-optimize](./prompt-cache-optimize/) | Prompt Caching 优化 |

## 使用方法

```bash
# 在 Claude Code 中使用
/claude "使用 product-verify skill 审查这个 PR"
/claude "使用 test-gen skill 为这个函数生成测试"
/claude "使用 security-check skill 检查安全问题"
```

## 安装

```bash
# 克隆到本地
git clone https://github.com/354685856-sn/claude-code-skills.git

# 复制到 .claude 目录
cp -r claude-code-skills/* ~/.claude/skills/
```

## 参考

- [Thariq Shihipar - How We Use Skills](https://www.linkedin.com/pulse/lessons-from-building-claude-code-how-we-use-skills-thariq-shihipar-iclmc)
- [Thariq Shihipar - Prompt Caching Is Everything](https://x.com/trq212/status/2024574133011673516)

## 许可证

MIT
