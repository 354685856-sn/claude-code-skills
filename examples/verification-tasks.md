# Verification Tasks

Use these tasks to check whether the most important skills produce useful, concrete output.

## product-verify

Task:

```text
Review a checkout page change. The new implementation adds a coupon field, updates total price after apply, and shows an error if the coupon is invalid.
```

Pass criteria:

- Checks functional behavior, invalid coupon behavior, loading state, and mobile layout.
- Separates blocking issues from suggestions.
- Gives concrete fixes instead of vague UX comments.

## test-gen

Task:

```text
Generate tests for a function that calculates shipping fee by region, cart total, and user membership level.
```

Pass criteria:

- Includes normal cases, boundary cases, and invalid inputs.
- States the test framework assumption.
- Gives a command to run the tests.

## security-check

Task:

```text
Review an API endpoint that accepts a file upload and stores metadata in a database.
```

Pass criteria:

- Checks file type validation, size limits, path traversal, authentication, authorization, logging, and dependency risks.
- Flags severe issues separately.
- Gives fix steps that an engineer can apply.

## code-review

Task:

```text
Review a session management module that creates, refreshes, and revokes access tokens.
```

Pass criteria:

- Prioritizes correctness and security.
- Finds token expiry, revocation, race condition, and error handling risks.
- Does not spend most of the review on style.

## prompt-cache-optimize

Task:

```text
Optimize an agent prompt that includes stable rules, tool definitions, project files, user request, and recent logs.
```

Pass criteria:

- Moves stable instructions before volatile context.
- Keeps user request and logs late in the prompt.
- Mentions append-only message ordering.
- Explains how the structure protects cache reuse.
