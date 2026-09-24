# Flight search for Claude Code

`/flights` searches Google Flights through the [fli](https://github.com/punitarani/fli) MCP server,
using the [van4oza/gflights-mcp-skill](https://github.com/van4oza/gflights-mcp-skill) playbook.

- `.claude/skills/flights/` — the skill (update with `npx skills update`)
- `.mcp.json` — runs `fli-mcp` via `uvx` (requires [uv](https://docs.astral.sh/uv/)); no API key needed
- `.claude/settings.json` — auto-enables the server and raises MCP output/timeout limits for large results

Cloud sessions need `www.google.com` allowed in the environment's network access.

Prices come from an unofficial Google Flights API; confirm on the airline's site before booking.
