# 04 ROS diagrams

## Goal

Support `"type": "risk"` for threat modeling, risk assessment and mitigation mapping.

## Scope

- [ ] Model: threats/causes → risks → consequences, with mitigations linked to risks
- [ ] Optional likelihood and impact per risk
- [ ] Graph builder showing the causal chain left to right and mitigations clearly attached
- [ ] Review criteria: clear causal chain, readable consequences, visible mitigations
- [ ] Example `diagrams/ros/union-risk/`

## Acceptance criteria

- [ ] Every risk without a mitigation is flagged in review
- [ ] Example renders and passes review above threshold
- [ ] Tests for schema and builder

## Dependencies

- [v1 Core pipeline](../v1-core/)

## Out of scope

- Risk scoring workflows or integration with external ROS tools
