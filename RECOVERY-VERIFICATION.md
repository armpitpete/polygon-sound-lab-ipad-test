# Sound Lab v0.1.7 — Polygon SEQ v4.8.6 Recovery Verification

**Verified:** 24 October 2026  
**Purpose:** Document the historical link between the frozen standalone Sound Lab and the 24-sound factory bank used in the Polygon SEQ v4.8.6 development candidate. This record makes **no software changes**.

## Authoritative sources

| Artifact | Identification |
| --- | --- |
| Sound Lab repository | `armpitpete/polygon-sound-lab-ipad-test` |
| Frozen Sound Lab source | `index.html` at Git commit [`17f785152f096887eea92d77d832aa345a05fd9c`](https://github.com/armpitpete/polygon-sound-lab-ipad-test/commit/17f785152f096887eea92d77d832aa345a05fd9c) |
| Frozen Sound Lab SHA-256 | `087fe68aa84bf569f60d2a158171b4acc3185d555d94c862fcc0b07d3ba43b63` |
| Recovered Polygon source | `Polygon-v4.8.6-Sound-Lab-Factory-Replacement.html` |
| Recovered Polygon SHA-256 | `5de0c6f8237e939960c5c0e971cecec979ee6af397149a528011479b0683c96f` |
| Factory manifest | `Sound-Lab-Factory-Manifest.json`, preserved with the original Polygon v4.8.6 development candidate |
| Standalone Sound Lab acceptance | [Full Windows PC final acceptance](SOUND-LAB-v0.1.7-FINAL-ACCEPTANCE.md), 15 October 2026 |

The original Sound Lab `index.html` was extracted as the **original Git blob**. Git for Windows can convert LF to CRLF in the checkout, which changes the working-file SHA-256. The unchanged original Git blob matches the frozen SHA-256 above.

## Reproducibility check

On the connected Windows PC, the recovered Sound Lab v0.1.7 original source was executed in Microsoft Edge. Its read-only `PolygonSoundLabQA` interface was used to render the original 24 factory presets through the original `renderSound` and `wavBlob` functions. Original factory parameters and deterministic seeds from `FACTORY_ROWS` were retained. The rendered WAV bytes and PCM frame counts were compared against the 24 entries of the recovered Polygon v4.8.6 manifest.

| Test | Result |
| --- | --- |
| Sound Lab original Git-blob SHA-256 | **PASS** — exact |
| Preset names and order | **PASS** — 24/24 |
| Sound categories | **PASS** — 4 engines × 6 presets |
| Generated PCM frame counts | **PASS** — 24/24 |
| Generated WAV SHA-256 values | **PASS** — **24/24 exact matches** |
| JavaScript page errors during this comparison | **None observed** |

The recovered factory categories are:
- **Sub Pulse:** Gravitation, Quasar Thud, Bent Sub, Soft Impact, Rubber Pulse, Deep Current
- **Metallic:** Distant Bell, Alloy Spark, Machine Tooth, Ice Chime, Rust Plate, Glass Engine
- **Noise:** Ion Spray, Static Stitch, Sand Blast, Tape Spit, Wind Crack, Dust Particle
- **Organic:** Hollow Seed, Wet Wood, Membrane Drift, Liquid Knock, Elastic Twig, Waterstone

The exact 24/24 regenerated WAV matches establish that the recovered Polygon v4.8.6 factory WAVs correspond to the frozen Sound Lab v0.1.7 synthesis implementation and preset data.

## Recovery archive and boundaries

The recovered original Polygon v4.8.6 candidate, sound manifest, extracted 24 WAVs, later v4.8.8 reference candidates, source comparisons, and test evidence were preserved in a **local Windows recovery package** named `Polygon-4.8.6-AUTHENTICATED-RECOVERY.zip`. That package is *not* added to this standalone Sound Lab repository, because the Polygon sequencer has separate ownership and acceptance criteria.

Previously recorded Polygon v4.8.6 Windows regression evidence (27/27 groups) remains historical: the original detailed test definitions were not recovered. Fresh tests do not prove that that specific historical suite was rerun. Human acceptance of the **integrated Polygon v4.8.6** remains separate from the standalone Sound Lab's existing Windows PC final PASS.

**Change-control boundary:** The existing Sound Lab v0.1.7 source, DSP algorithms, factory preset settings, recorded audio characteristics, and previous acceptance records remain frozen. This verification does **not** authorise additional Polygon SEQ integration, modification of its accepted percussion mechanism, or Live performance engine development.

## Correction to recovery process

The GitHub repository and its accepted history should have been searched **before** treating the original Sound Lab source as missing. Its discovery resolves the original source/provenance gap. Future recovery inventories must include project repositories and commit history at the start, alongside local and archived files.
