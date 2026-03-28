# Soc Ops

Soc Ops is a FastAPI + Jinja2 social bingo app built for in-person mixers, team offsites, and workshops.
Players explore the room, match people to prompts, and race to complete five in a row.

## Why This Project

- Fast to run locally and easy to demo in a live session.
- Clean Python structure for teaching architecture and testing.
- Designed for AI-assisted development workflows with Copilot.

## What You Can Do

- Start a new game with a fresh bingo board.
- Mark matched prompts directly from the game screen.
- Track win conditions with game logic covered by tests.
- Use it as a hands-on lab for prompt and multi-agent workflows.

## Tech Stack

- Backend: FastAPI
- Templates: Jinja2
- Frontend: HTML, CSS utilities, HTMX
- Test and lint: Pytest, Ruff
- Runtime: `uv`

## Quick Start

1. Install dependencies:

```bash
uv sync
```

2. Run the app:

```bash
uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

3. Run tests:

```bash
uv run pytest
```

4. Run lint:

```bash
uv run ruff check .
```

## Project Structure

- `app/`: FastAPI app, game logic, models, and services
- `templates/`: Jinja2 pages and components
- `app/static/`: CSS and JavaScript assets
- `tests/`: API and game logic tests
- `workshop/`: markdown lab content for local/offline use

## Workshop Guide

Follow the guided lab to learn and extend the project:

| Part | Title |
|------|-------|
| [**00**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview) | Overview & Checklist |
| [**01**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=01-setup) | Setup & Context Engineering |
| [**02**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=02-design) | Design-First Frontend |
| [**03**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=03-quiz-master) | Custom Quiz Master |
| [**04**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=04-multi-agent) | Multi-Agent Development |

Lab guides are also available in [workshop/](workshop/) for offline reading.

## Contributing

If you want to improve gameplay, visuals, or workshop content, open an issue or PR.
Please review [CONTRIBUTING.md](CONTRIBUTING.md) before submitting changes.
