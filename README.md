# Resonance Intelligence Core (RIC)

Deterministic inference substrate.  
A coherence-locked alternative to probabilistic AI.  
Replayable, signed bundles with claims and provenance.

---

## Website
[resonanceintelligencecore.com](https://resonanceintelligencecore.com)  
Download signed demo bundles (Contract, Compliance).  
Verify locally with the CLI.

---

## Quick Start

```bash
# 1. Clone this public repo
git clone https://github.com/devinbostick/ric-core-public
cd ric-core-public

# 2. Verify a demo bundle (requires jq installed)
./dist/cli/verify.js artifacts/contract-bundle.json --json | jq .

Expected output:

{
  "signature": { "status": "verified", "alg": "ed25519" },
  "bundleHash": "...",
  "graphHash": "..."
}

What makes RIC different
	•	Deterministic — no probabilities, no stochastic drift
	•	Legality enforced — PAS, CHORDLOCK, TEMPOLOCK, AURA_OUT
	•	Replayable — outputs are reproducible across runs
	•	Signed — Ed25519-signed bundles with provenance

⸻

Contents
	•	artifacts/contract-bundle.json → PASS (valid contract demo)
	•	artifacts/compliance-bundle.json → FAIL (conflict demo)
	•	README.md → Overview and instructions

⸻

Contact

For licensing or collaboration:
devin.bostick@codesintelligence.com
resonanceintelligencecore.com
