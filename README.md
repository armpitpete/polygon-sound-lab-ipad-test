# Polygon Sound Lab — iPad Safari browser test

**Current experimental version: v0.1.2 (Noise HPF/LPF)**

[Open the test instrument](https://armpitpete.github.io/polygon-sound-lab-ipad-test/)

## What changed in v0.1.2

- The Noise voice now has **High-pass** and **Low-pass** cutoff controls (20 Hz to 18 kHz).
- The confusing **Filter offset** control has been removed from the Noise editor. Its old saved `pitch` value is retained internally for loading older presets, but no longer affects Noise audio.
- HPF cuts low-frequency noise; LPF cuts high-frequency noise. Both filters act on the entire Noise signal.
- The two filters can cross. This can make the sound extremely quiet, intentionally; the UI warns when they cross.
- Filtering uses two cascaded one-pole stages for each band edge (about 12 dB/octave).
- Stored `hpfHz` and `lpfHz` are part of new custom Noise presets; older presets import with 25 Hz HPF and 14 kHz LPF defaults.
- Sub Pulse, Metallic, and Organic PCM remains unchanged compared with v0.1.1.

## Evidence and scope

**76/76 automated tests PASS** (46 regression, 30 targeted HPF/LPF tests); tested on desktop Chromium. Spectral testing measured independent high/low frequency attenuation; WAV export and preset round-trips passed. Real iPad Safari audio, downloads, and storage persistence **not yet accepted**.

This is a public, isolated experimental prototype, not a release of the main Polygon SEQ drum sequencer. No other project or sequencer code is modified.

The website uses browser-local storage where available. **Export a JSON library backup** for custom sounds, especially before clearing Safari site data.

## Previous releases

- [v0.1.1 — pitched-noise repair](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1.1/)
- [v0.1 — original](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1/)

Exact v0.1.2 HTML SHA-256: `625a1bee89500d884cdb4983b2c50bced7703db6131fdbbc09e30d885d99e49c`.
