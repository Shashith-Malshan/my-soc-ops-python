---
description: Testing instructions for deterministic pytest coverage in this project.
applyTo: "tests/**/*.py"
---

# Testing Instructions

## Scope

- Keep tests focused on observable behavior, not implementation details.
- Extend existing files before creating new test modules.
- Prefer deterministic test data and avoid flaky timing assumptions.

## Coverage Expectations

- Add tests when changing endpoint behavior or game rules.
- Cover both success and error/edge paths for changed logic.
- Keep API tests aligned with current response contracts.

## Style

- Follow existing pytest style and fixture patterns in tests/.
- Keep assertions specific and readable.
- Avoid unnecessary mocking if direct calls are fast and stable.

## Verification

- Run `uv run pytest` after test changes.
- Keep test runtime reasonable by scoping new cases to changed behavior.
