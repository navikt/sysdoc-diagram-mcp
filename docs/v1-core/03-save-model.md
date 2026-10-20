# 03 save_model

## Goal

Persist the semantic model as `diagram.json`.

## Scope

- [ ] Tool input: `diagram_id`, `model`
- [ ] Validate model before writing
- [ ] Write via storage module (path validation from v0)
- [ ] Stable, pretty-printed JSON with deterministic key order for clean Git diffs
- [ ] Atomic write (temp file + rename)
- [ ] Output: path to `diagram.json`

## Acceptance criteria

- [ ] Saving the same model twice gives byte-identical files
- [ ] Invalid `diagram_id` or model is rejected without writing
- [ ] Unit tests

## Dependencies

- [02 create_diagram](02-create-diagram.md)
- [v0 storage layout](../v0-foundation/03-diagram-storage-layout.md)

## Out of scope

- Git commits
