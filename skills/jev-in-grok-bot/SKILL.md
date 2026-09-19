---
name: Jev in Grok Bot
description: >-
  Use when wiring TypeSafe Jev into Grok Bot — decision gates, claim verify,
  context screen, confidence routing, or publishing a Jev Desk template.
---
# Jev in Grok Bot

## When
You need TypeSafe **Jev** inside Grok Bot: decision gates, claim verify vs evidence, context screen before untrusted text enters context, confidence routing, or a public Jev Desk template.

## What Jev is
TypeSafe System One model: state + typed questions → structured answers (no free-form generation). Primitives: **Choice**, **Score**, **Noul**. Docs: https://docs.typesafe.ai · confidence routing: https://docs.typesafe.ai/patterns/confidence-routing.md · agent skill: https://docs.typesafe.ai/agent-skill.md

## Three lanes (full toolkit)
1. **Decision gate** — before send/pay/merge/cancel: Choice (act/hold/ask) + Score (risk) + Noul (policy satisfied?). Route by confidence: auto / review / block.
2. **Claim verify** — claims + evidence → verified | contradicted | unsupported (citation_check cookbook).
3. **Context screen** — untrusted web/tool text → pass | review | block | skip. Filter only, not a hard security boundary (llm_guardrails cookbook).

## Setup
1. TypeSafe API key as `TYPESAFE_API_KEY`.
2. Custom Jev MCP (not a marketplace plugin): install via the host's Add MCP flow with the published `jev-mcp` / TypeSafe MCP package and env `TYPESAFE_API_KEY`. Confirm the exact package command with current TypeSafe docs.
3. Keep questions + thresholds in one reviewable policy (memory or skill).
4. Optional: TypeSafe coding-agent skill from https://github.com/typesafe-ai/skills

## Operating rules
- Never invent probabilities or confidence.
- Teach while doing: show question, state summary, verdict, confidence, route.
- External side effects still need explicit human Approve unless a pre-agreed high-confidence auto policy says otherwise.
- Prefer a dated ledger of gate decisions over chat-only magic.
- Public templates: name TypeSafe/Jev MCP in log memory; never pack API keys or custom MCP configs.

## Done when
Clear verdict + confidence + route (auto / review / block), or a public Jev Desk template staged without secrets.
