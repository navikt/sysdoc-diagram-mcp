# 03 review_diagram

## Goal

Expose diagram review as an MCP tool.

## Context

The client LLM does the visual analysis of the PNG. The server supplies the image, metrics and criteria.

## Scope

- [ ] Tool input: `diagram_id`
- [ ] Return PNG as image content, layout metrics and the applicable criteria
- [ ] Optional second step/tool to submit the client's review so it is validated against the review model
- [ ] Combine metric-based and visual issues into one `score` + `issues` result
- [ ] Store latest review next to the diagram (e.g. `review.json`) if useful for the loop

## Acceptance criteria

- [ ] Copilot can review the `union` example and return a score with issues
- [ ] Output matches the readme format: `{ "score": 8, "issues": [] }`
- [ ] Tests for metric-only review path

## Dependencies

- [02 Layout metrics](02-layout-metrics.md)

## Out of scope

- Applying fixes (see v3)
