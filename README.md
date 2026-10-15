# Polygon Sound Lab — Isolated test edition

[Open the current browser Sound Lab](https://armpitpete.github.io/polygon-sound-lab-ipad-test/)

**Current version: v0.1.6 — workflow and playback-mixer repair.** Windows browser automated validation passed; whole-instrument human acceptance pending.

## Four approved synthesis voices

The sound engines and all 24 factory presets are unchanged from the individually accepted v0.1.5:

- **Noise:** White/Pink/Brown colours, HPF, LPF, optional band-pass, envelope and texture.
- **Metallic:** Six accepted FM percussion presets.
- **Sub Pulse:** Six accepted low-frequency/percussive presets.
- **Organic:** Six accepted modal/resonator presets.

All four v0.1.5 listening PASS records remain in this repository. All factory and representative custom digital audio renders, as well as individual exported WAV files, were tested against the frozen source.

## v0.1.6 repairs

1. **Playback headroom:** All live playback goes through one gain and bounded soft-limiter bus. Rapid retriggers, including 48 simultaneous source triggers, passed offline output peak tests below unity. This changes live monitor level; the exported mono WAV sound is unchanged.
2. **Protect unsaved edits:** Selecting another sound or importing a preset for the edited voice opens a modal offering **Save changes / Discard changes / Cancel**. Save on a factory draft creates a new custom sound, while Save on an existing custom draft updates that sound.
3. **Per-voice unsaved names:** Sound names remain available when switching across the four kit slots.
4. **Stored-bank recovery:** If one record is corrupt, Sound Lab keeps the valid sounds available and warns that recovery is required. You can download the exact original stored bytes, then explicitly repair. Before repair, the app writes and verifies a separate recovery copy in browser storage. It never automatically overwrites the original damaged library.

## Tests and release boundary

**18/18 Windows repair/regression groups passed** (9 Chrome and 9 Edge). This includes 24 factory PCM identity comparisons plus 4 Noise variants, per-voice WAV byte comparisons, draft handling, corrupt-library repair, and a 48-trigger limiter stress test (peak **0.751052**).

This is **not formal whole-instrument acceptance by the user**. Complete personal Windows PC testing and explicit PASS remain required. iPad Safari support is secondary.

Four active kit assignments are intentionally temporary and reset at page reload. Saved custom sounds persist in browser storage where permitted. Back up JSON files before clearing browser data. Saved libraries are separate for different website origins or browsers.

**Main Polygon percussion versions and workflows are untouched.** There is no automatic integration; exported WAVs can be imported as samples using Polygon's existing sample controls.

## Archived versions

- [v0.1.5 — individually accepted four voices](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.5/)
- [v0.1.4 — White/Pink/Brown initial](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.4/)
- [v0.1.3 — Band-pass](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.3/)
- [v0.1.2 — HPF/LPF](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.2/)
- [v0.1.1 — Unpitched Noise](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.1/)
- [v0.1 — Initial](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1/)

Accepted frozen v0.1.5 SHA-256: `5db837ad358ec7c8d4bc586db52c5ec66470ae5a25204f9fd8c620f31fd2c43b`

v0.1.6 SHA-256: `d5862f6a233c29fea677925b9f6687920089d2a6ae2034adce122500a16f57c7`
