# Usage Examples

This file gives one practical usage example for every skill in this repository.

## context7

Use when you need current documentation before implementing with a library or API.

```text
使用 context7 skill 查 Next.js App Router 最新的 metadata API，并给出官方文档链接和最小示例。
```

Expected output:

- Core API summary
- Version or compatibility notes
- Minimal code example
- Reference links

## product-verify

Use after a feature is implemented to check whether behavior matches the product requirement.

```text
使用 product-verify skill 审查这个登录页改动，重点检查错误提示、加载状态、移动端布局和可访问性。
```

Expected output:

- Passed items
- Product issues
- Blocking UX problems
- Concrete fixes

## data-fetch

Use when a debugging task needs logs, metrics, user feedback, or production evidence before changing code.

```text
使用 data-fetch skill 汇总最近 24 小时登录失败相关日志，按错误类型和影响用户数分组。
```

Expected output:

- Data source and time range
- Key findings
- Suspected root cause
- Recommended next actions

## gsd

Use when a task is large enough to need a plan, execution log, and review pass.

```text
使用 gsd skill 把“重构支付回调处理”拆成计划、执行、审查三个阶段，并列出验收标准。
```

Expected output:

- Task plan
- Execution checklist
- Review checklist
- Acceptance criteria

## code-review

Use for a focused code review that prioritizes correctness, security, maintainability, and performance.

```text
使用 code-review skill 审查 src/auth/session.ts，重点看 token 过期、权限绕过和错误处理。
```

Expected output:

- Severe issues
- Recommended improvements
- Good patterns to keep

## test-gen

Use when code changed and you need targeted tests rather than generic coverage.

```text
使用 test-gen skill 为 calculateDiscount 函数生成单元测试，覆盖边界值、非法输入和四舍五入规则。
```

Expected output:

- Test file path
- Test cases added
- Test command
- Test result summary

## doc-gen

Use when README, API docs, or code comments need to match the current implementation.

```text
使用 doc-gen skill 根据 src/api/orders.ts 更新订单 API 文档，包含请求参数、响应字段和错误码。
```

Expected output:

- Generated or updated files
- API surface covered
- Documentation gaps

## security-check

Use before merging sensitive code, auth code, payment code, upload code, or user input handling.

```text
使用 security-check skill 审查文件上传模块，重点看路径遍历、MIME 校验、大小限制和日志脱敏。
```

Expected output:

- Passed checks
- Warnings
- Severe issues
- Fix steps

## env-setup

Use when a project needs repeatable local setup, dependency checks, or tool version alignment.

```text
使用 env-setup skill 检查这个仓库的 Node 版本、包管理器、环境变量和测试命令是否完整。
```

Expected output:

- Current environment status
- Completed setup actions
- Manual setup items
- Verification command

## superpowers

Use when a problem needs architecture thinking, option comparison, or a deeper solution design.

```text
使用 superpowers skill 设计一个 Obsidian + Claude Code 的长期记忆系统，给出 3 个方案并推荐一个。
```

Expected output:

- Clear recommendation
- Option comparison
- Risks and tradeoffs
- Implementation plan

## prompt-cache-optimize

Use when prompt or agent context structure affects latency, cost, or cache hit rate.

```text
使用 prompt-cache-optimize skill 优化这个 agent system prompt，把稳定内容和动态内容分层。
```

Expected output:

- Current cache risks
- Suggested prompt layout
- Stable prefix recommendations
- Expected improvement
