# 03 Capability maps

## Goal

Support `"type": "capability"` for product, platform and business capabilities.

## Scope

- [ ] Model: hierarchical capabilities (domain → capability → sub-capability), optional status/maturity
- [ ] Graph builder producing a balanced, nested layout (clusters or grid)
- [ ] Review criteria: balanced hierarchy, readable grouping, minimal clutter
- [ ] Example diagram under `diagrams/capability/`

## Acceptance criteria

- [ ] Hierarchies of at least three levels render readably
- [ ] Example passes review above threshold
- [ ] Tests for hierarchy validation

## Dependencies

- [v1 Core pipeline](../v1-core/)

## Out of scope

- Linking capabilities to systems or teams
