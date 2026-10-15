# Polygon Sound Lab v0.1.7 — Full Instrument Acceptance

**FINAL PASS — USER ACCEPTED / WINDOWS PC / FROZEN BASELINE**

- Acceptance date: **15 October 2026**
- Approved version: **Polygon Sound Lab v0.1.7**
- Frozen `index.html` SHA-256: `087fe68aa84bf569f60d2a158171b4acc3185d555d94c862fcc0b07d3ba43b63`
- Live standalone version: https://armpitpete.github.io/polygon-sound-lab-ipad-test/
- Human decision: user's explicit **"PASS"** following the final Windows PC acceptance checklist and the completed Windows technical review.
- Supporting report: `SOUND-LAB-v0.1.7-WINDOWS-ACCEPTANCE-REPORT.md` (30/30 Windows Chrome/Edge automated test groups passed; public HTTPS bytes matched the tested source).

## Scope accepted

Whole **standalone** Sound Lab instrument as presented and tested on Windows PC:

- Four independent, accepted synthesis engines: **Sub Pulse, Metallic, Noise and Organic**.
- **24 factory sounds** with their accepted sound-design controls and predictable sound playback.
- Noise's deliberately **dirty/granular Texture** implementation introduced in v0.1.7; earlier subjective PASS recorded in `NOISE-v0.1.7-ACCEPTANCE.md`.
- Sound editor, per-voice draft names, safe Play All/retrigger mixing, Preview and Stop.
- Save/Discard/Cancel before replacing edits; custom presets, updating, deleting and reloading.
- Browser-local sound library, editable individual JSON export/import, full JSON bank backup/import, and non-destructive damaged-bank recovery.
- **44.1 kHz 16-bit mono WAV export** and the tested Windows Chrome/Edge workflow.

The preceding individual engine acceptance records for Sub Pulse, Metallic and Organic remain in effect. Final Windows PC human acceptance is **now complete**, superseding the "human acceptance pending" state noted in the earlier technical evidence report.

## Release and change control

**Freeze v0.1.7.** Future functionality must be developed additively in a separate version or isolated experiment. Do not alter the accepted sounds or their workflow without fresh, explicit approval and comparative verification.

**Important scope boundary:** This PASS **does not** authorise integrating Sound Lab into Polygon SEQ, changing Polygon's established percussion sound engine, altering frozen Polygon versions, or promoting any separate melodic experiment. A potential integration must be separately scoped, tested, and explicitly authorised. Current sample reuse through manual WAV export already works.

Kit assignments remain temporary on page reload by the accepted design; saved individual custom sounds persist per browser-origin/profile when local storage is available, with JSON export for portable backups. iPad remains secondary to Windows PC and is not covered by this Windows acceptance.

**Authoritative acceptance:** this record and the unchanged SHA-256 source, not inference from automated tests alone.
