# Claude Code Skills

Custom Claude Code skills for repeatable agent harness workflows: code review, testing, security checks, documentation, context optimization, product verification, and task execution.

## Why

Claude Code becomes more useful when repeatable work is captured as skills instead of rewritten as one-off prompts.

This repository collects reusable skills for common software engineering and AI agent workflows. The long-term goal is to turn practical experience into small, portable instructions that can be installed, tested, improved, and shared.

## Skills

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

## Repository layout

Each skill follows the same basic shape:

```text
skill-name/
└── SKILL.md
examples/
├── usage-examples.md
└── verification-tasks.md
```

`SKILL.md` is the entrypoint Claude Code reads when the skill is selected. Keep each skill focused, concrete, and easy to verify.

## Examples and verification

- [Usage examples](./examples/usage-examples.md) gives one practical call pattern for every skill.
- [Verification tasks](./examples/verification-tasks.md) gives small tasks for checking whether key skills produce concrete output.

## Install

```bash
git clone https://github.com/354685856-sn/claude-code-skills.git
mkdir -p ~/.claude/skills
cp -R claude-code-skills/* ~/.claude/skills/
```

## Usage examples

```bash
/claude "使用 product-verify skill 审查这个 PR"
/claude "使用 test-gen skill 为这个函数生成测试"
/claude "使用 security-check skill 检查安全问题"
```

## Quality checklist

Before adding or changing a skill:

- The skill has one clear job.
- The instructions are operational, not just conceptual.
- The expected input and output are obvious.
- The skill avoids unnecessary context and long generic guidance.
- The skill can be tested on a real task.

## Roadmap

- [x] Add examples for every skill.
- [x] Add verification tasks for key skills.
- [ ] Add a compatibility note for current Claude Code skill directory conventions.
- [ ] Split broad skills into smaller, verifiable workflows where needed.
- [ ] Publish a first release after the skill set is reviewed.

## References

- [Thariq Shihipar - How We Use Skills](https://www.linkedin.com/pulse/lessons-from-building-claude-code-how-we-use-skills-thariq-shihipar-iclmc)
- [Thariq Shihipar - Prompt Caching Is Everything](https://x.com/trq212/status/2024574133011673516)

## License

MIT
