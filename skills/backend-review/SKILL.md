---
name: backend-review
description: Review backend code for correctness, security, and maintainability.
---

# Backend Review Skill

## Scope

Use this skill when reviewing backend code (Node.js, Java, Python, Go, .NET).

## Review Checklist

1. Correctness: Validate logic, null/edge cases, and error handling.
2. Security: Check auth/authz, input validation, injection risks, and secrets leakage.
3. Data safety: Validate transaction boundaries, idempotency, and migration compatibility.
4. Performance: Flag N+1 queries, blocking calls, and unbounded loops.
5. Observability: Ensure logs, metrics, and trace context are present on critical paths.
6. Test quality: Verify unit/integration tests cover happy path and failure path.

## Output Format

- Findings first, ordered by severity.
- Include file path and suggested fix.
- Keep summary concise.
