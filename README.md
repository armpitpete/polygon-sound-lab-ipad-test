# Polygon Sound Lab — iPad Safari test

[Open Sound Lab (latest)](https://armpitpete.github.io/polygon-sound-lab-ipad-test/)

**Current prototype: v0.1.1** — isolated, browser-based four-voice experimental percussion synthesis. This is not an accepted Polygon SEQ release.

## v0.1.1 Noise repair (15 October 2026)

Following iPad listening feedback, the Noise voice has been corrected to produce stochastic noise only. Two accidental or unwanted pitched sine-wave components were present in v0.1:
- A sine tone in the grit component.
- A second sine tone in the low-texture transient.

Both were replaced with seeded random noise. The Noise pitch slider now reads **Filter offset**; the saved JSON parameter key remains 'pitch' for compatibility. The other three voices' PCM outputs are unchanged, sample for sample.

Technical validation in automated Chromium: 46/46 existing checks PASS; 21/21 repair-specific checks PASS. All six Noise presets have much lower coherent tone peaks in numerical spectrum checks. Actual iPad listening and Safari export/storage behaviour still require device acceptance.

**Old custom Noise presets** are still loadable, but their sound changes in v0.1.1 because the oscillator is removed. Back up your library JSON before experimenting.

### Archived original

[v0.1 original HTML](https://armpitpete.github.io/polygon-sound-lab-ipad-test/archive/v0.1/)

## Use and limitations

1. Open the site in Safari on iPad and press Play on the Noise voice.
2. Move Filter offset, Tone and Texture; compare all six Noise presets.
3. Save a sound and export WAV; test Safari download to Files.
4. Back up custom presets as JSON; clearing browser site data can remove saved presets.

Sound synthesis executes entirely in the browser, with no external runtime libraries. No changes have been made to the existing Polygon percussion sequencer or melodic experiment.

Verified deployed v0.1.1 SHA-256 expected: `56ef3ef497444da936ef2ffb25918b84245f1f7afcb3990b3adfe34e32b3a0fe`.
