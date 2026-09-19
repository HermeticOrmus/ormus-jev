# Three lanes

## 1. Decision gate
Before a consequential action (send, pay, merge, cancel spend):
- **Choice** — act / hold / ask
- **Score** — risk or fit (0–1 from Jev, never invented)
- **Noul** — policy satisfied?

Route by confidence: auto / review / block. External side effects still need human Approve unless a pre-agreed high-confidence policy says otherwise.

## 2. Claim verify
Inputs: claim text + evidence snippets.  
Outputs: verified | contradicted | unsupported.  
Use for contest claims, outbound copy, and repo README numbers.

## 3. Context screen
Untrusted web/tool text → pass | review | block | skip.  
This is a filter, not a security boundary. Low confidence → human.

## Ledger
Prefer a dated local ledger of gate decisions over chat-only magic.
