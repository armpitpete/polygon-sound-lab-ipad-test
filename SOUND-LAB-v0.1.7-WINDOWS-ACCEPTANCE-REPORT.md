# Polygon Sound Lab — Windows PC whole-instrument acceptance evidence

**Review date:** 15 October 2026  
**Build:** Sound Lab v0.1.7  
**Decision:** **TECHNICAL PASS / HUMAN WINDOWS PC ACCEPTANCE PENDING**  
**Frozen HTML SHA-256:** `087fe68aa84bf569f60d2a158171b4acc3185d555d94c862fcc0b07d3ba43b63`  
**Production test link:** https://armpitpete.github.io/polygon-sound-lab-ipad-test/

## Automated Windows acceptance

All tests ran on the connected **Windows 10 PC**, using locally installed Google Chrome and Microsoft Edge. Browser contexts were isolated from the user's ordinary browser profiles and saved presets.

| Evidence | Outcome |
|---|---|
| Complete v0.1.7 browser regression on Chrome | **10/10 PASS** |
| Complete v0.1.7 browser regression on Edge | **10/10 PASS** |
| Separate Windows public HTTPS end-to-end checks | **10/10 PASS** |
| **Total** | **30/30 test groups PASS** |

Covered playback of each voice, kit playback/Stop, 48 overlapping trigger safety, 24 factory presets, sample parity with accepted baselines, Noise Texture across all colours and factory variants, custom sound creation/updating, Save/Discard/Cancel, per-voice draft names, browser restart persistence, reproducible 44.1 kHz mono 16-bit WAV exports, JSON preset/library backup and import, corrupt-bank non-destructive recovery, responsive widths, Chrome to Edge bank transfer, and storage safety.

The **published HTTPS page is byte-identical** to the v0.1.7 accepted-source file by SHA-256. No code changes were made during final acceptance testing.

## Voice-specific listening approvals

- **Noise v0.1.7:** PASS; user explicitly approved its dirty/granular Texture.
- **Metallic:** PASS; engine unchanged since approval.
- **Sub Pulse:** PASS; engine unchanged since approval.
- **Organic:** PASS; engine unchanged since approval.

These separate sound approvals remain valid. Whole-instrument human acceptance has **not** been claimed.

## What still needs the user's PC test

Open the live link in an ordinary Chrome or Edge window on the Windows PC. Use comfortable speaker/headphone volume.

1. **Playback:** Click each voice's Play and **Play all four**, then **Stop playback**. Confirm no unpleasant overload/distortion, clicks, or unexpectedly loud output.
2. **Sound edit:** Select Noise, choose Ion Spray, and preview **Texture 0% versus 100%**. Confirm the dirtier sound is still satisfactory on PC speakers/headphones.
3. **Protect edits:** Select Sub Pulse, change Pitch and Sound name, then choose another preset. Verify **Cancel** preserves the draft and **Discard** loads the selected preset. Try changing voices and returning to verify the draft name survives.
4. **Save/reopen:** Save a temporary custom sound, reload the page, and confirm it is still available in **My saved sounds**. Delete this temporary sound afterwards if desired.
5. **Exports:** Export one WAV and play it using a Windows audio player. Export a custom-library JSON backup. Confirm the downloaded files can be found and opened.

User to reply **PASS** if the complete PC workflow is acceptable, or **REPAIR** with the specific issue. Do not interpret this technical report or any automation as the user's personal sign-off.

## Boundaries

Kit assignments remain temporary by design; individual custom sounds persist. Local storage is specific to the browser origin/profile, and JSON backup should be used for portability. This is a standalone sound-design/export instrument; **no automatic integration into the established Polygon SEQ percussion sequencer is authorised or performed**.

If human Windows PC acceptance passes, the next decision is whether existing WAV export is sufficient or a separately reviewed, additive integration is warranted. Preserve all established Polygon percussion versions and their accepted workflow.
