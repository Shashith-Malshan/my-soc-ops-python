# Copilot Instructions

## Project Context
- This is a Python web app using FastAPI with Jinja2 templates.
- Core app code lives in `app/`.
- HTML templates live in `templates/`.
- Static assets live in `app/static/`.
- Tests live in `tests/`.

## Coding Standards
- Keep changes minimal and focused on the user request.
- Preserve existing naming, code style, and structure.
- Prefer readable, explicit Python over clever one-liners.
- Add short comments only when logic is not obvious.
- Avoid introducing new dependencies unless clearly needed.

## Backend Guidelines
- Keep endpoint handlers thin; move logic to `app/game_logic.py` or service modules.
- Validate inputs at API boundaries.
- Keep data models in `app/models.py` consistent with existing patterns.
- Avoid breaking response shapes used by templates and tests.

## Template and UI Guidelines
- Reuse existing template components in `templates/components/` when possible.
- Follow utility classes defined in `app/static/css/app.css`.
- Do not invent utility class names that do not exist; add them to CSS first if needed.
- Preserve accessibility basics: labels, button semantics, and readable text contrast.

## Testing and Quality
- Add or update tests for behavior changes.
- Keep test scope focused and deterministic.
- Prefer extending existing test files before creating new ones.

## Checklist
- [ ] int
- [ ] build
- [ ] test

## Suggested Commands
- Lint: `uv run ruff check .`
- Test: `uv run pytest`
- Run app: `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000`
