# Ormus Jev resources

Open teaching pack for **TypeSafe Jev** (System One) as Ormus uses it inside Grok Bot and coding agents.

> Study seed: [@AIGuide_](https://x.com/AIGuide_/status/2101119480361361685) → [article](https://x.com/i/article/2100744524951932928) · Canonical docs: [docs.typesafe.ai](https://docs.typesafe.ai)

## What Jev is

A typed decision model: state + questions → **Choice**, **Score**, **Noul** (not free-form chat). Confidence is returned by the model; never invent it.

## Ormus three lanes

1. **Decision gate** — before send / pay / merge / cancel  
2. **Claim verify** — claims vs evidence  
3. **Context screen** — untrusted text before it enters context (filter, not a hard security boundary)

See [docs/three-lanes.md](docs/three-lanes.md).

## Quick paths

| Path | File |
|------|------|
| Grok Bot setup | [docs/grok-bot-setup.md](docs/grok-bot-setup.md) |
| Public skill | [skills/jev-in-grok-bot/SKILL.md](skills/jev-in-grok-bot/SKILL.md) |
| Example packs | [examples/](examples/) |
| Study notes | [docs/study-notes.md](docs/study-notes.md) |

## Gold Hat

Empower installers. Never pack API keys. Name `TYPESAFE_API_KEY` + Jev MCP in installer memory only. See [GOLD_HAT.md](GOLD_HAT.md).

## Related

- TypeSafe skills: https://github.com/typesafe-ai/skills  
- Ormus Jev Desk bot template (scrubbed, no keys) — ask Diego / Auric for export after Approve  

## License

MIT. Jev / TypeSafe product terms remain with TypeSafe AI.
