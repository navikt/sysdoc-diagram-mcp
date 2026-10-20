# 01 Layout hints in model

## Goal

Let the semantic model carry intent that improves layout, without encoding coordinates.

## Context

Review fixes must change the JSON, never DOT/SVG/PNG. The model therefore needs semantic hints the builder can act on.

## Scope

- [ ] Define hints: `importance` (`primary`, `secondary`), `group`, optional `order` within a role
- [ ] Graph builder maps hints to DOT (e.g. primary → larger/centered, group → cluster, order → node ordering)
- [ ] Keep hints optional and backwards compatible (bump `schema_version` if needed)

## Acceptance criteria

- [ ] `"importance": "primary"` on Union visibly changes rendering
- [ ] Grouping consumers produces a cluster
- [ ] Golden tests for each hint

## Dependencies

- [v2 Review](../v2-review/)

## Out of scope

- Absolute positioning
