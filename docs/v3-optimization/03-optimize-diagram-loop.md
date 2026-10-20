# 03 optimize_diagram loop

## Goal

Run model → render → review → improve until the diagram is good enough.

## Scope

- [ ] Tool input: `diagram_id`, `threshold` (default e.g. 8), `max_iterations` (default e.g. 5)
- [ ] Stop on `score >= threshold`, max iterations, or no improvement
- [ ] Keep the best-scoring model, not just the last one
- [ ] Record history (iteration, score, issues, changes)
- [ ] Decide how the loop drives client-side review (MCP prompt guiding Copilot, or metric-only mode)

## Acceptance criteria

- [ ] Loop always terminates
- [ ] Final `diagram.json` and artifacts correspond to the best score
- [ ] Test with metric-only review that improves a deliberately bad model

## Dependencies

- [02 improve_model](02-improve-model.md)

## Out of scope

- Organization-specific scoring (see v4)
