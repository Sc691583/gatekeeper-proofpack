# Claims (Evidence-First)

C01 — Fail-Closed Default  
- Unpermitted action attempts are denied with a receipt (PASS/FAIL evidence).

C02 — Controlled Allow (Safe Path)  
- A safe allowlisted operation can be allowed and executed under enforced constraints (receipt-based).

C03 — Tamper Detection  
- Evidence tampering is detected deterministically by offline verification (expected FAIL).

C04 — Anchor Integrity  
- Anchor chain integrity holds for baseline and fails under mutation suite (reorder/splice/truncate).

Verification is offline and reproducible via `run_all.sh` inside the release bundle.
