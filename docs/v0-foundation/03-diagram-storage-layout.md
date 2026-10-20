# 03 Diagram storage layout

## Goal

Define how diagrams are stored on disk and in Git.

## Context

All diagrams live under `diagrams/<type>/<id>/` with `diagram.json`, `diagram.dot`, `diagram.svg` and `diagram.png`. Only the JSON is edited by hand.

## Scope

- [ ] Storage module resolving paths from `type` and `diagram_id`
- [ ] Validate `diagram_id` (e.g. `^[a-z0-9][a-z0-9-]{0,63}$`) to prevent path traversal
- [ ] Configurable root directory (env var, default `./diagrams`)
- [ ] Decide whether generated artifacts are committed or ignored, and document it
- [ ] Function to regenerate all artifacts from `diagram.json`

## Acceptance criteria

- [ ] Paths outside the root directory are rejected
- [ ] Deleting `.dot`, `.svg`, `.png` and regenerating gives identical output
- [ ] Unit tests for path resolution and validation

## Dependencies

- [02 Semantic model schema](02-semantic-model-schema.md)

## Out of scope

- Git operations (commit/push) from the server
