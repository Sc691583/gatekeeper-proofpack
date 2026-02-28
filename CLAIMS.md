# Gatekeeper ProofPack — Claims (Proof-Only)

This repository does **not** contain implementation details.

## Proven (offline, reproducible PASS/FAIL)

### C1 — Deterministic Posture Transitions (NORMAL ↔ LOCKDOWN)
- When hazards are present, posture becomes **LOCKDOWN** and execution is **fail-closed** (`allow_execute=false`).
- When hazards clear, posture returns to **NORMAL** (`allow_execute=true`).

Evidence is delivered as an **offline release bundle** (ProofPack).  
Verification produces a single **overall PASS/FAIL** verdict and exits with code `0` on PASS.
