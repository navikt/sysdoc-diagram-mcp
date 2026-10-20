# 02 Semantic model schema

## Goal

Define the semantic graph model (`diagram.json`) as the single source of truth.

## Context

The model captures architectural intent, not layout. It must support multiple diagram types, starting with `dataflow`. See "Separate Semantics From Rendering" in the readme.

## Scope

- [ ] Pydantic models with a discriminated union on `type` (`dataflow` first; `integration`, `architecture`, `capability`, `risk` reserved)
- [ ] Dataflow model with roles: `sources`, `processors`, `storage`, `consumers`
- [ ] Nodes accept a plain string or an object (`name`, optional `importance`, `group`, `label`)
- [ ] Explicit `edges` (`from`, `to`, optional `label`); define how edges are inferred when omitted
- [ ] Unique node names and validation that edges reference existing nodes
- [ ] `schema_version` field
- [ ] Export JSON Schema to `schema/diagram.schema.json`

## Acceptance criteria

- [ ] The readme dataflow example validates
- [ ] Invalid models (unknown type, dangling edge, duplicate node) fail with clear messages
- [ ] JSON Schema export is generated from code and checked in CI

## Dependencies

- [01 Project setup](01-project-setup.md)

## Out of scope

- Layout hints beyond `importance`/`group` (see [v3 layout hints](../v3-optimization/01-layout-hints-in-model.md))
