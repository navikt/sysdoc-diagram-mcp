# 02 Architecture and trust boundaries

## Goal

Support `"type": "architecture"` with platforms, applications, infrastructure and trust zones.

## Scope

- [ ] Model: zones (nested allowed), components assigned to zones, flows between components
- [ ] Graph builder rendering zones as clusters with visible borders
- [ ] Highlight flows crossing trust boundaries
- [ ] Review criteria: visible boundaries, logical grouping, clear primary flow
- [ ] Example diagram under `diagrams/architecture/`

## Acceptance criteria

- [ ] Boundary-crossing flows are visually distinct
- [ ] Example renders and passes review above threshold
- [ ] Tests for nested zones

## Dependencies

- [v1 Core pipeline](../v1-core/)

## Out of scope

- Full threat modeling (see [ROS diagrams](04-ros-diagrams.md))
