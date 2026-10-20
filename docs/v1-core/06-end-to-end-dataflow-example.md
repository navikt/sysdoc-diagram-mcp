# 06 End-to-end dataflow example

## Goal

Prove the v1 pipeline with the `union` dataflow example from the readme.

## Scope

- [ ] Add `diagrams/dataflow/union/diagram.json` with SAP, Kafka, Union, Snowflake, Grafana and Slack
- [ ] Generate DOT, SVG and PNG through the tools
- [ ] End-to-end test: create → save → generate → render
- [ ] Short usage section in readme showing the Copilot prompt and result

## Acceptance criteria

- [ ] A user can describe the architecture in Copilot and get an SVG and PNG without writing DOT
- [ ] Deleting generated files and rerunning reproduces them
- [ ] End-to-end test passes in CI

## Dependencies

- [05 render_diagram](05-render-diagram.md)

## Out of scope

- Review and optimization
