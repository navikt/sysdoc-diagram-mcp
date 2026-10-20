# 02 Layout metrics

## Goal

Compute deterministic layout metrics without an LLM.

## Context

Graphviz can output positions with `-Tjson`. These give objective input to the review.

## Scope

- [ ] Render layout as JSON alongside SVG/PNG
- [ ] Count edge crossings
- [ ] Detect overlapping nodes and labels
- [ ] Measure whitespace ratio and aspect ratio
- [ ] Check role ordering for dataflow (x-position of sources < processors < consumers)
- [ ] Map metrics to issues using the review criteria

## Acceptance criteria

- [ ] Metrics are deterministic for the same input
- [ ] Unit tests with crafted layouts (known crossings/overlaps)

## Dependencies

- [01 Review criteria](01-review-criteria.md)

## Out of scope

- Visual (image-based) analysis
