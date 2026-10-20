# 02 improve_model

## Goal

Apply review feedback to the semantic model.

## Scope

- [ ] Tool input: `model`, `review`, and proposed changes from the client
- [ ] Changes expressed as a constrained patch (e.g. JSON Patch limited to allowed paths)
- [ ] Rule-based fixes for known issue codes (e.g. "consumers should be grouped" → add `group`)
- [ ] Validate the updated model before returning
- [ ] Output: `{ "updated_model": {...} }` plus a summary of changes

## Acceptance criteria

- [ ] Never modifies DOT, SVG or PNG directly
- [ ] Patches that break the schema or remove nodes unintentionally are rejected
- [ ] Unit tests per rule-based fix

## Dependencies

- [01 Layout hints in model](01-layout-hints-in-model.md)

## Out of scope

- Running the loop (see [optimize_diagram](03-optimize-diagram-loop.md))
