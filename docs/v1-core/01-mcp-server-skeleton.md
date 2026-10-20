# 01 MCP server skeleton

## Goal

Run a minimal MCP server that GitHub Copilot can connect to.

## Context

Uses `FastMCP` from the `mcp` SDK over stdio.

## Scope

- [ ] Server entry point (`diagram-agent` console script)
- [ ] Tool registration pattern, one module per tool
- [ ] Consistent error handling: validation errors returned as tool errors, not crashes
- [ ] Logging to stderr (stdout is reserved for the protocol)
- [ ] Example `.vscode/mcp.json` for local use
- [ ] Expose the JSON Schema as an MCP resource

## Acceptance criteria

- [ ] Server starts and lists tools in VS Code
- [ ] MCP Inspector can call a placeholder tool
- [ ] Smoke test starting the server in-process

## Dependencies

- [v0 Foundation](../v0-foundation/)

## Out of scope

- HTTP transport and authentication
