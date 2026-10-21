# 01 Project setup

## Goal

Create a Python project skeleton for the MCP server.

## Context

The server is written in Python using the official `mcp` SDK. Graphviz is required as a system dependency for rendering.

## Scope

- [x] Initialize project with `uv` and `pyproject.toml` (Python 3.12+)
- [x] Add dependencies: `mcp`, `pydantic`
- [x] Add dev dependencies: `pytest`, `ruff`, `pyright` or `mypy`
- [x] Package layout: `src/diagram_agent/`, `tests/`
- [x] Document Graphviz installation (`dot` on `PATH`) in readme
- [x] CI workflow running lint, type check and tests (with Graphviz installed)
- [x] `.gitignore` for Python artifacts

## Acceptance criteria  

- [ ] `uv sync && uv run pytest` passes on a clean checkout
- [ ] `uv run ruff check` passes
- [ ] CI runs on pull requests

## Dependencies

None.

## Out of scope

- MCP tools (see v1)
