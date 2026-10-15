# Polygon Sound Lab — Noise v0.1.7 Listening Acceptance

**Status: PASS — NOISE v0.1.7 FROZEN**

- Date: 15 October 2026
- Version: Polygon Sound Lab v0.1.7
- User verdict: **"Pass, it's dirty, I like it."**
- Scope of verdict: the Noise engine's repaired, distinctly audible Texture control, retaining the user's preferred dirty / granular / irregular crackling character.
- Frozen source SHA-256: `087fe68aa84bf569f60d2a158171b4acc3185d555d94c862fcc0b07d3ba43b63`
- Browser prototype: https://armpitpete.github.io/polygon-sound-lab-ipad-test/

## Accepted Noise design

White / Pink / Brown noise; independent high-pass and low-pass filters; optional band-pass (centre and width); audible Texture from smoother noise at 0% to rougher granular sputtering/crackling at 100%; Attack, Decay and Level; presets and deterministic WAV export. No pitched oscillator in the Noise signal path.

The user specifically prefers the strong **dirty** character of the revised Texture. Do not silently smooth, weaken, equalise away, or otherwise redesign it. Any proposed change to this accepted sound must be isolated to a new version and reviewed through listening.

The v0.1.7 Windows Chrome and Edge regression run reported **20/20 test groups PASS**. The Sub Pulse, Metallic and Organic renders and WAV exports remained identical to v0.1.6; Noise at Texture 0% was identical, whereas nonzero Texture deliberately changed to address the previous inaudible control.

The old `NOISE-ACCEPTANCE.md` remains the historical v0.1.5 acceptance; this record supersedes it for the Noise DSP baseline.

## Scope boundaries

This is an explicit **human listening PASS for Noise Texture/Noise v0.1.7**, not acceptance of all v0.1.7 Sound Lab editing, storage and workflow behaviour on the user's primary Windows PC, nor permission to merge Sound Lab into the established Polygon percussion sequencer.

- Noise: PASS v0.1.7 — frozen.
- Metallic: PASS (unaltered from previous accepted version).
- Sub Pulse: PASS (unaltered from previous accepted version).
- Organic: PASS (unaltered from previous accepted version).
- Whole Sound Lab: Windows human usability acceptance outstanding.
- Existing Polygon SEQ percussion: untouched.

**Next stage:** Check complete Sound Lab usability on the user's Windows PC; proceed to full-instrument acceptance only after explicit approval.
