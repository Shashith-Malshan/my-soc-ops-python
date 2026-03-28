---
description: Python backend instructions for FastAPI routes, game logic, and service-layer changes.
applyTo: "app/**/*.py"
---

# Backend Python Instructions

## Architecture

- Keep route handlers in app/main.py thin and focused on HTTP concerns.
- Put gameplay rules and board/win logic in app/game_logic.py.
- Use service functions for orchestration and avoid duplicating logic across endpoints.

## Validation and Data Shape

- Validate user input at API boundaries.
- Preserve response shapes expected by templates and tests.
- Keep model usage aligned with patterns already used in app/models.py.

## Change Strategy

- Prefer small, targeted edits over broad refactors.
- Reuse existing helpers before adding new abstractions.
- Add short comments only where branching or state transitions are non-obvious.

## Safety Checks

- If behavior changes, update tests in tests/ to reflect the new contract.
- Avoid adding new dependencies unless absolutely necessary.
