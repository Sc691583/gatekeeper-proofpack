# Gatekeeper ProofPack (Proof-Only)

This repository contains a proof-only wrapper for offline, reproducible PASS/FAIL verification.

No internal implementation details are included (no architecture, endpoints, component lists, or operational procedures).
Only claims + offline verification entrypoint.

## Bundle availability
The proof bundle is **not published** in this repository.
Only a proof-only wrapper + claims + offline verification entrypoint are public.

A release bundle can be provided **on request**.
Published artifacts include **SHA256 hashes** under `RELEASES/`.

## How to verify (offline)
1) Obtain the ProofPack release bundle (`GK_PROOFPACK_V1_RELEASE_*.tar.zst`) via the provided channel.
2) Extract:
   - `tar -I 'zstd -T0 -d' -xf GK_PROOFPACK_V1_RELEASE_*.tar.zst`
3) Run:
   - `./run_all.sh`
4) Expected output:
   - `overall: PASS` and exit code `0`

## What is proven
See `CLAIMS.md`.
