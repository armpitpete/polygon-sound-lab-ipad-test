# Polygon Sound Lab — iPad browser test

[Open the latest Sound Lab](https://armpitpete.github.io/polygon-sound-lab-ipad-test/)

**Current version: v0.1.4 — isolated experimental prototype, not part of the accepted Polygon drum sequencer.**

## Noise channel — listening test

Choose the Noise voice and select **Noise colour**:

- **White** — even-spectrum static and sharp hiss.
- **Pink** — approximately 3 dB less energy per higher octave, softer and more balanced.
- **Brown** — approximately 6 dB less energy per higher octave, deep rumbles.

The three colours use seeded, deterministic noise generators. **No pitched oscillator** has been added. The existing High-pass, Low-pass, optional Band-pass, Texture, Attack, Decay and Level controls remain available. Tone stays hidden for Noise and stays active on the other three synth voices.

An older Noise preset without the new `noiseColour` key defaults to White. Imported presets still work. Custom colour choice is preserved in saved JSON presets and in WAV rendering. On changing colour, you must save or update the preset if you want to keep your change.

Existing six factory Noise sounds retain their original output when White is selected. The Sub Pulse, Metallic and Organic voices render unchanged.

**Automated Chromium testing:** 154/154 checks passed, including measured frequency spectra, DSP determinism, clipping, old preset import, JSON/WAV export, and 430px layout. Human iPad Safari listening and file persistence acceptance are outstanding.

**This is the final planned Noise development revision until listening review.** Do not add further Noise features or integrate it with the main drum sequencer until accepted.

## Persistence and older versions

Custom presets are stored in your browser where permitted. Back up your library as JSON; browser data removal can erase saved sounds. Some iPad browsers may restrict WAV/JSON downloads.

- [v0.1.3 (band-pass)](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.3/)
- [v0.1.2 (high-pass/low-pass)](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.2/)
- [v0.1.1 (remove unwanted tonal oscillators)](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.1/)
- [v0.1 initial](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1/)

Current HTML SHA-256: `03aa96ce51db659e4439c959645867f7b7d3216dda9134529caef9e46205ade6`.
