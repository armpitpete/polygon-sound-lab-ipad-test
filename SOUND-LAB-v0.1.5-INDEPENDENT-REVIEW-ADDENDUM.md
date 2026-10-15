# Polygon Sound Lab v0.1.5 — Independent Review Addendum

**Review date:** 15 October 2026  
**Decision:** REPAIR (standalone whole-instrument PASS withheld); freeze four accepted voices and all factory presets.  
**Reviewed source SHA-256:** `5db837ad358ec7c8d4bc586db52c5ec66470ae5a25204f9fd8c620f31fd2c43b`.

## Independent verification

Read the published source and the complete Windows instrument review. Native Windows Chrome isolated-profile checks independently reconfirmed unsaved-edit loss and exposed a further recovery failure. The previous **29/29 positive workflow checks** remain valid; they are not evidence that the separate defect checks passed.

| Priority | Finding | Evidence | Repair acceptance |
|---|---|---|---|
| P1 | Play All lacks sufficient mix headroom | Four synchronized defaults sum to a peak of **1.793889** in the offline sample calculation, above 1.0 unity; four BufferSourceNodes connect straight to AudioDestinationNode | Implement **mixer/bus-only** gain staging and safe multi-trigger output; test worst-case combinations and retrigger overlaps at the output, with no unapproved changes to per-voice DSP/PCM or one-voice WAV files |
| P1 | Dirty preset replaced without prompt | 204-Hz unsaved Pitch reset to **84 Hz** on selecting factory Bent Sub, and the status simply says preset loaded | A clear, accessible Save / Discard / Cancel workflow; Cancel preserves all draft fields; apply guard to all replacements, including imported matching-engine sounds |
| P2 | Unsaved name lost when switching kit slots | `chooseVoice()` always assigns `soundName.value=v.name`, whereas slider edits remain in `slots[]` | Keep a distinct per-slot editable draft name through voice switching; Save, Update and WAV export use the draft name appropriately |
| P2 | One invalid stored preset hides the whole sound library | After inserting one invalid record next to one valid persisted custom sound and reloading, the app displays **0 custom sounds** and incorrectly reports storage unavailable; original two raw JSON entries remain in localStorage | Preserve original raw data, show a truthful recovery warning, allow backup/recovery of valid entries without silent overwrite, and test clean reload/import afterwards |
| Deferred | Whole-kit save/recall | Kit assignments intentionally reset on reload; individual sounds persist and JSON bank transfer works Chrome → Edge | Separate product decision, not a release repair requirement |

**Clipping qualification:** a summed float peak above 1.0 proves inadequate headroom and a risk of downstream clipping, but not audible distortion on the user's output device. Repair must account for repeated simultaneous triggers, not only the four default samples.

## Scope discipline and release gates

1. Create **isolated v0.1.6** for mixer safety, draft preservation/guard, and stored-bank recovery. Do not add synthesis features, new kit formats or sequencer integration.
2. Assert **sample-for-sample parity** for all 24 accepted factory voice renders and representative custom presets, including all three Noise colours. Validate the four original voice algorithms and exported mono WAVs remain identical to v0.1.5.
3. Exercise all four repairs on Windows Chrome and Edge, with save/cancel paths, corrupt-bank backups/recovery, library portability, dense/repeated triggers, keyboard interaction, and no horizontal overflow.
4. Obtain explicit **human Windows PC whole-instrument acceptance**. Individual voice PASS records remain valid independently; iPad testing is secondary.
5. Only then decide whether separate Sound Lab WAV export is sufficient or whether integration is even necessary. Never modify the established Polygon sequencer without an independent decision.

No Sound Lab code or existing percussion code was modified by this review.
