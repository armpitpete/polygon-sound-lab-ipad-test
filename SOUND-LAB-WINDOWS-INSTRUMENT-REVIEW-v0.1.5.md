# Polygon Sound Lab v0.1.5 — Windows Complete Instrument Review

**2026-10-15 | Decision: REPAIR / NO-GO for full instrument acceptance and integration**

**Source integrity:** HTML SHA-256 `5db837ad358ec7c8d4bc586db52c5ec66470ae5a25204f9fd8c620f31fd2c43b`. Native Windows Chrome and Edge tested in isolated browser contexts. Published HTTPS page opened in Windows Chrome and matched the same SHA-256. Normal browser profiles and saved user presets were not modified.

## Tests that passed

**29/29 automated Windows browser checks PASS**, covering four-slot voice editing/playback, 24 factory sounds, kit assignments, Play All/Stop, custom preset saving/updating/duplication/deletion/reload, sound-name validation, editable JSON and complete bank export/import, WAV 44.1 kHz 16-bit mono export and deterministic re-export, invalid JSON/schema/member rejection, protection against HTML-like preset names, temporary kit behaviour, 1366/1920/430px layouts, storage-denied fallback, and independent Windows Edge Organic WAV export.

Cross-browser portability: one custom sound of each engine was exported from Chrome and successfully imported into a fresh Edge context (**4/4**). Noise waveform redraw during 12 low-pass changes: **median 7.9 ms**, maximum **9.1 ms**, on tested Windows hardware.

## Release risks found

1. **P1: Potential Play All clipping.** Peak of the four synchronously summed default voices measured **1.794** against unity full scale **1.0**. Sources are mixed without master attenuation or limiting. This establishes insufficient headroom, not confirmed audible distortion. Repair only the kit mixer/bus; do not change individual accepted sound renders or single-voice WAVs.
2. **P1: Silent loss of unsaved edits.** Choosing another factory preset discards modified Pitch (demonstrated using 204 Hz) without a warning. Add Save/Discard/Cancel or equivalent clear guarded transition.
3. **P2: Draft sound name lost on slot switching.** A name typed before Save disappears when changing voices and returning, unlike slider edits. Preserve name in per-slot draft state.
4. **Documented limitation, not a defect:** Four kit sound assignments reset on page reload. Individual custom presets persist. Full kit save/recall is not yet a feature; requires separate product decision.

Browser local storage is origin-specific and may be cleared; custom bank JSON export/import is validated. Windows automation does **not** mean user acceptance of the complete instrument, human-perceived sound quality, or iPad Safari behaviour.

## Controlled next stage

Hold whole-instrument PASS and native Polygon integration. Propose an isolated **v0.1.6 workflow/mixing-only repair** of the three issues. Preserve frozen Noise, Metallic, Sub Pulse and Organic v0.1.5 DSP and factory presets unchanged, and prove sample-for-sample audio parity for every single voice. Final Windows PC user acceptance required before any integration decision. iPad is secondary.

**Review altered no synthesis code.** Voice-specific approval records remain valid; they do not constitute full Sound Lab acceptance.
