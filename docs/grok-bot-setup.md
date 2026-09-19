# Jev in Grok Bot (setup)

1. Get a TypeSafe API key → store as env `TYPESAFE_API_KEY` (never commit).
2. Add custom Jev MCP via the host Add MCP flow (`jev-mcp` / TypeSafe package per current docs). Confirm install command in https://docs.typesafe.ai.
3. Save policy questions + thresholds in bot memory or this skill pack.
4. Optional: TypeSafe coding-agent skill from https://github.com/typesafe-ai/skills
5. Public templates: name the service in log memory; **never** pack keys or MCP configs into share json.

Smoke: run a trivial Choice question; confirm typed answer + confidence appears; route low confidence to review.
