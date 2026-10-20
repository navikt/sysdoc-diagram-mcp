# 05 render_diagram

## Goal

Render `diagram.dot` into `diagram.svg` and `diagram.png` with Graphviz.

## Scope

- [ ] Call `dot` via `subprocess` with an argument list (no shell)
- [ ] Timeout and size limits
- [ ] Clear error if Graphviz is missing or DOT is invalid (include stderr)
- [ ] Configurable PNG DPI
- [ ] Tool input: `diagram_id`; output: paths to SVG and PNG
- [ ] Optionally return the PNG as image content for preview

## Acceptance criteria

- [ ] Readme example renders SVG and PNG
- [ ] Invalid DOT returns a tool error, not a crash
- [ ] Integration test (skipped when `dot` is missing locally, required in CI)

## Dependencies

- [04 generate_graph](04-generate-graph.md)

## Out of scope

- Review of the rendered image (see v2)
