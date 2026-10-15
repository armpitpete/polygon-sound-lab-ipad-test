# Polygon Sound Lab — isolated browser test

[Open latest Sound Lab](https://armpitpete.github.io/polygon-sound-lab-ipad-test/)

**CURRENT ACCEPTED RELEASE: v0.1.7 — FULL WINDOWS PC INSTRUMENT PASS / FROZEN.** All four engines and the complete standalone Windows workflow are user accepted. See [final acceptance record](SOUND-LAB-v0.1.7-FINAL-ACCEPTANCE.md). Polygon SEQ percussion is unchanged; integration is NOT approved.

## Noise Texture correction

v0.1.6 Texture was almost inaudible. In v0.1.7, Noise Texture gradually introduces stronger, irregular, pitchless granular/sputtering modulation, while White/Pink/Brown colour sources, the existing low-pass/high-pass/band-pass filters and other controls remain available.

Use **Noise → Texture** at **0%** and **100%**, pressing **Preview voice** after each adjustment. Existing playing samples do not update live. Presets with nonzero Texture will sound different; export a JSON library backup before switching versions.

Across six Noise factory presets and three colours, Texture 0% versus 100% waveform correlation decreased from roughly 0.901–0.959 to 0.464–0.756.

- 240/240 targeted deterministic DSP checks passed.
- 20/20 Windows Chrome and Edge browser test groups passed.
- All Sub Pulse, Metallic, Organic factory PCM and WAV renders remain unchanged; Noise at Texture 0% remains unchanged.
- Sound Lab v0.1.6 usability repairs (safe mixer, unsaved edit guard, draft names and damaged library recovery) remain intact.

**Acceptance:** The user explicitly approved v0.1.7 Noise Texture: "Pass, it's dirty, I like it." Preserve that pronounced dirty/granular character. See [Noise v0.1.7 acceptance](NOISE-v0.1.7-ACCEPTANCE.md). Metallic, Sub Pulse and Organic retain their earlier accepted audio. Full standalone Sound Lab Windows PC acceptance is now recorded in [FINAL ACCEPTANCE](SOUND-LAB-v0.1.7-FINAL-ACCEPTANCE.md). Any Polygon integration still requires a separate decision.

## Previous revisions

- [v0.1.6 — complete workflow/mixer repairs](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.6/)
- [v0.1.5 — individually accepted voice reference](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.5/)
- [v0.1.4 — White/Pink/Brown](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.4/)
- [v0.1.3 — band-pass](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.3/)
- [v0.1.2 — high-pass/low-pass](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.2/)
- [v0.1.1 — no unwanted pitched noise](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.1/)

**v0.1.7 SHA-256:** `087fe68aa84bf569f60d2a158171b4acc3185d555d94c862fcc0b07d3ba43b63`

Voice-specific approvals and prior instrument reviews remain available in this repository. The standalone HTML uses no network resources and no external scripts. Personal presets are stored in the current browser origin where permitted; maintain exported JSON backups.
