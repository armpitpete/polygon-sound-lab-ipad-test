# Polygon Sound Lab — iPad browser test

[Open the latest Sound Lab](https://armpitpete.github.io/polygon-sound-lab-ipad-test/)

**Current version: v0.1.5 — isolated technical repair, awaiting real iPad listening acceptance.**

## Pink / Brown sound correction

Listening feedback found Pink and Brown too similar in v0.1.4. That version mixed a separate bright white-noise grit signal **after** colour filtering, which masked the distinction.

In **v0.1.5**, the complete noise excitation, including Texture/grit, is coloured before the existing high-pass, low-pass and optional band-pass filters.

- White source and its factory presets: unchanged PCM output.
- Sub Pulse, Metallic and Organic: unchanged PCM output.
- Pink: more upper-frequency content than Brown.
- Brown: much more bass-dominant, with reduced high-frequency hiss.
- No pitched oscillator added, and no new controls.

**Validation:** 81/81 targeted DSP checks passed, and narrow-screen Chromium UI smoke test passed. Upper-frequency contrast between Pink/Brown rose from approximately 0.7–2.4 dB in v0.1.4 to approximately 5.2–6.1 dB over all six factory Noise presets.

**Listening test:** Compare Pink and Brown using identical filter settings and Texture values. On the iPad, use headphones if possible because small speakers attenuate the bass that distinguishes Brown noise. If the sounds still feel too close, note the exact preset and listening equipment.

**Saved sounds:** Older preset JSON remains supported. Previously saved Pink and Brown sounds will render differently; export your preset bank JSON backup first. Browser local storage can be cleared by Safari.

**Noise development remains on hold pending listening acceptance.** Do not change the accepted Polygon percussion sequencer to integrate this experimental prototype.

## Previous versions

- [v0.1.4 — first White/Pink/Brown addition](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.4/)
- [v0.1.3 — band-pass](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.3/)
- [v0.1.2 — high-pass and low-pass](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.2/)
- [v0.1.1 — remove unwanted pitched oscillators](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.1/)
- [v0.1 — original](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1/)

v0.1.5 SHA-256: `5db837ad358ec7c8d4bc586db52c5ec66470ae5a25204f9fd8c620f31fd2c43b`.
