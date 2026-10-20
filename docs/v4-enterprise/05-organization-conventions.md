# 05 Organization conventions

## Goal

Let organizations define their own styling and review rules.

## Scope

- [ ] Config file (e.g. `diagram-conventions.json`) with styles per node kind, colors, fonts
- [ ] Extra review rules (e.g. required labels, naming patterns, mandatory trust zones)
- [ ] Config validated with Pydantic and exposed as an MCP resource
- [ ] Graph builders and review read conventions; defaults apply when absent

## Acceptance criteria

- [ ] Changing the config changes rendering without touching `diagram.json`
- [ ] Custom review rule produces issues in `review_diagram`
- [ ] Tests with and without config

## Dependencies

- [v2 Review](../v2-review/)
- Diagram types in this folder

## Out of scope

- UI for editing conventions
