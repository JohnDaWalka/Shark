# Copilot Coding Agent Instructions

## Repository purpose and scope
- Shark is a cross-platform Python project that will evolve into complex chatbot integrations (e.g., Perplexity- or Grok-style experiences).
- Primary language: Python 3 with standard library utilities in `src/platform_utils.py`.
- Preserve Windows, macOS, and Linux compatibility; avoid platform-specific regressions.

## How to work in this repo
- Favor small, well-scoped changes with clear acceptance criteria.
- Keep code typed and documented; match existing docstring style.
- Do not hardcode secrets or tokens; rely on environment variables when needed.
- Leave Sourcery feedback in place and keep CI workflows unchanged unless explicitly requested.

## Setup and validation
- Create a virtual environment and install dependencies:
  - `python -m venv .venv && source .venv/bin/activate` (Unix/macOS) or `.venv\Scripts\activate` (Windows)
  - `python -m pip install -r requirements.txt` (currently no third-party packages, but keeps environments aligned)
- There are no automated tests yet. If you add tests, prefer `pytest` in a `tests/` directory and keep them cross-platform.
- For quick manual validation: `python -m compileall src` and run `python -m src.platform_utils` to ensure platform info prints without errors.

## Issue and PR guidance
- Include the target files, expected behavior, and validation steps in issues.
- Keep PRs minimal; reference the issue being addressed and mention any manual validation performed.
