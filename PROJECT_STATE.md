# Project State — Polygon Sound Lab

**Last reviewed:** 24 October 2026  
**This repository:** https://github.com/armpitpete/polygon-sound-lab-ipad-test  
**Default branch:** `main`  
**Operating contract:** [PROJECT_EXECUTION_CONTRACT.md](PROJECT_EXECUTION_CONTRACT.md)

## Status and accepted baseline
- **Product:** Isolated four-voice browser synthesiser; this is *not* the core Polygon SEQ repository.
- **Latest accepted standalone release:** **v0.1.7**, Windows PC human PASS, frozen 15 October 2026. See [final acceptance](SOUND-LAB-v0.1.7-FINAL-ACCEPTANCE.md).
- **Source file:** `index.html` at commit `17f785152f096887eea92d77d832aa345a05fd9c`.
- **Authoritative Git blob SHA-256:** `087fe68aa84bf569f60d2a158171b4acc3185d555d94c862fcc0b07d3ba43b63`. A Windows checkout with CRLF may have a different *working-file* hash; compare the original blob.
- **Accepted engines:** Sub Pulse, Metallic, Noise, Organic, six factory presets each (24 total). Strong dirty/granular Noise Texture is accepted and must be preserved.
- **Accepted features:** sound editor, preset/draft management, offline WAV export, Windows workflow as documented in the final acceptance file. Browser kit assignments are intentionally temporary.
- **Frozen:** original DSP, presets, source, human acceptance record. Development requires an isolated version plus explicit approval.

## Provenance for Polygon SEQ
- **Recovered original core candidate:** `Polygon-v4.8.6-Sound-Lab-Factory-Replacement.html` from the connected Windows PC.
- **v4.8.6 SHA-256:** `5de0c6f8237e939960c5c0e971cecec979ee6af397149a528011479b0683c96f`.
- **Recovered factory bank:** 24 original WAVs and `Sound-Lab-Factory-Manifest.json`.
- **Independent link:** v0.1.7's original factory rendering reproduced **24/24 WAV SHA-256 values** and **24/24 PCM frame counts**. See [recovery verification](RECOVERY-VERIFICATION.md).
- **Local evidence:** Windows `Documents\PolygonSEQ-Recovery-2026-10-24\Polygon-4.8.6-AUTHENTICATED-RECOVERY.zip`, plus QA JSON. This archive belongs to the Polygon SEQ recovery effort and is not silently released or committed into Sound Lab.
- **Core Polygon SEQ status:** v4.8.6 source and bank technically recovered; core human integration approval is **not** implied. v4.9 layout/Live preview is a separate unapproved candidate. Existing percussion remains untouched.
- **Other known repo:** https://github.com/armpitpete/polygon-melodic-ipad-test — isolated melodic experiments only. Do not treat it as Polygon SEQ core.

## Evidence / acceptance gates
1. Standalone Sound Lab frozen release: **PASS — human PC acceptance documented**.
2. v4.8.6 source authenticity and 24 audio parity: **PASS — hashes verified**.
3. Repetition of original historical Polygon 27-group suite: **NOT VERIFIED — original detailed suite unavailable**.
4. Direct integrated v4.8.6 listening and user usability approval: **OPEN**.
5. Core four-workspace and future Live performance release: **OPEN; separate authorisation**.

## Next tasks
- Preserve recovery and parity proof; don't regenerate 24 sounds.
- For core Polygon SEQ work, first locate the actual current working source and its project ledger, use existing recoveries, then test Windows workflows and obtain explicit approval only where required.
- Reconcile status against task-specific evidence, not previous aggregate claims.
- Keep these records current when an accepted decision, source location, test result or blocker changes.
