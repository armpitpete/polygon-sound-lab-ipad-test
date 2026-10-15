# Polygon Sound Lab — iPad test

[Open latest Sound Lab](https://armpitpete.github.io/polygon-sound-lab-ipad-test/)

Current version: **v0.1.3** (experimental, not accepted on physical iPad or integrated with Polygon SEQ).

## Noise improvements

- Independent high-pass (HPF) and low-pass (LPF) controls.
- Optional band-pass (BPF): tick **Enable band-pass**, then change its centre frequency and bandwidth in octaves.
- Removed redundant Tone from Noise. Tone remains available to the Sub Pulse, Metallic and Organic voices.
- Unpitched, seeded noise only; no tonal oscillator in the Noise path.
- Existing Noise preset JSON remains importable; the old pitch/tone keys are retained for format compatibility, but no longer modify Noise audio.
- This intentionally changes how some existing Noise presets sound.

Presets are stored in your browser locally. Export JSON backups; clearing site data may remove locally saved presets. WAV download and iPad Safari persistence require on-device tests.

The Band-pass filter is serial and optional: the sound goes through HPF, LPF, then (when enabled) BPF. Filters can produce very low volume if frequency bands do not overlap.

Technical tests (Chromium): **112/112 PASS**; sub/metal/organic PCM byte identical to v0.1.2. Audio needs human listening evaluation.

## Previous revisions

- [v0.1.2 (HPF/LPF)](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.2/)
- [v0.1.1 (remove unwanted Noise pitches)](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.1/)
- [v0.1 initial](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1/)

Current HTML SHA-256 `ca78baeeb60fd4ad48ac2d9c5b034ba344f68c43e4f354eaefbc51e274669060`.

This repository is a separate test deployment. No change to the accepted Polygon drum sequencer or melodic prototypes.
