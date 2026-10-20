# 01 Review criteria

## Goal

Define what a good diagram is, per diagram type, and how it is scored.

## Context

See "Quality Guidelines" in the readme.

## Scope

- [ ] Common checks: edge crossings, overlapping labels, whitespace, visual balance, readability
- [ ] Type-specific checks (dataflow: sources left, processing center, consumers right)
- [ ] Scoring scale 0–10 with weighting between checks
- [ ] Review result model: `score`, `issues` (each with `code`, `message`, optional `node`)
- [ ] Store criteria as data so they can be extended in v4

## Acceptance criteria

- [ ] Criteria documented and available as an MCP resource or prompt
- [ ] Review result model validated with Pydantic

## Dependencies

- [v1 Core pipeline](../v1-core/)

## Out of scope

- Organization-specific rules (see [v4 conventions](../v4-enterprise/05-organization-conventions.md))
