# 04 generate_graph

## Goal

Convert `diagram.json` into `diagram.dot`.

## Context

Architecture knowledge stays in the model; layout rules live in the graph builder. Start with the `dataflow` type.

## Scope

- [ ] Graph builder interface with one implementation per diagram type
- [ ] Dataflow builder: `rankdir=LR`, role columns via `rank=same` (sources → processors → storage → consumers)
- [ ] Edge inference when the model has no explicit edges
- [ ] Escape node names and labels safely for DOT
- [ ] Deterministic output (stable ordering)
- [ ] Tool input: `diagram_id`; output: path to `diagram.dot`

## Acceptance criteria

- [ ] Readme example produces equivalent DOT to the readme snippet
- [ ] Names with quotes, spaces or special characters produce valid DOT
- [ ] Golden-file tests

## Dependencies

- [03 save_model](03-save-model.md)

## Out of scope

- Other diagram types (see v4)
- Layout hints (see v3)
