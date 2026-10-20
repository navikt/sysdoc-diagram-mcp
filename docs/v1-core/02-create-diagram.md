# 02 create_diagram

## Goal

Create a semantic graph model from a natural language description.

## Context

The MCP client LLM translates text into a model. The server provides the schema and validates the result.

## Scope

- [ ] Tool input: `description`, optional `type`, optional `diagram_id`, and a `model` proposed by the client
- [ ] Tool description includes clear instructions and a reference to the schema resource
- [ ] Validate the model; return validation errors so the client can retry
- [ ] Derive `diagram_id` from description when missing (slugified)
- [ ] Output: `{ "diagram_id": ..., "model": {...} }`

## Acceptance criteria

- [ ] Prompt "Show the flow between SAP, Union and Snowflake" produces a valid dataflow model via Copilot
- [ ] Invalid models return actionable errors
- [ ] Unit tests for validation and id derivation

## Dependencies

- [01 MCP server skeleton](01-mcp-server-skeleton.md)

## Out of scope

- Server-side LLM calls (MCP sampling is a later option)
- Persisting the model (see [save_model](03-save-model.md))
