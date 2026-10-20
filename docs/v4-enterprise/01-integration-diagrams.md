# 01 Integration diagrams

## Goal

Support `"type": "integration"` for APIs, event brokers and enterprise integrations.

## Scope

- [ ] Model: systems, interfaces (REST, event, file, batch), brokers/topics, directional edges with protocol labels
- [ ] Graph builder with distinct shapes for systems, APIs and brokers
- [ ] Review criteria: clear producer/consumer direction, brokers centered
- [ ] Example diagram under `diagrams/integration/`

## Acceptance criteria

- [ ] Example renders and passes review above threshold
- [ ] Schema, builder and criteria covered by tests

## Dependencies

- [v1 Core pipeline](../v1-core/) (v2/v3 for review and optimization)

## Out of scope

- Generating diagrams from OpenAPI or AsyncAPI specs
