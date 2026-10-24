# Acceptance and Change-Control Record

**Updated:** 24 October 2026.

## Accepted / frozen
| Scope | Decision | Evidence |
| --- | --- | --- |
| Standalone Sound Lab v0.1.7, all four engines and 24 factory sounds | **USER PASS / FROZEN** | [Final Windows acceptance](SOUND-LAB-v0.1.7-FINAL-ACCEPTANCE.md), 15 October 2026 |
| Sound Lab v0.1.7 Noise Texture | **USER LISTENING PASS / FROZEN** | [Noise acceptance](NOISE-v0.1.7-ACCEPTANCE.md) |
| v0.1.7 source original blob | **VERIFIED** | SHA-256 `087fe68aa84bf569f60d2a158171b4acc3185d555d94c862fcc0b07d3ba43b63` |
| Sound Lab → Polygon SEQ v4.8.6 factory bank provenance | **TECHNICAL PASS** | [24/24 exact WAV parity verification](RECOVERY-VERIFICATION.md) |

## Not accepted by the above
| Scope | Status | Outstanding decision/test |
| --- | --- | --- |
| Integrated Polygon SEQ v4.8.6 product | **TECHNICAL SOURCE RECOVERED; HUMAN ACCEPTANCE OPEN** | Windows music/listening and usability review; old full 27-group suite not recovered |
| Polygon v4.9 four-workspace integration preview | **UNAPPROVED** | Owner's Windows visual and workflow acceptance |
| Functional Live performance engine | **NOT AUTHORISED** | Separate scope and owner decision |
| iPad performance/release | **SECONDARY; NOT IMPLIED** | Separate platform evidence if/when prioritised |
| Sound Lab DSP or 24-sound bank modifications | **NOT AUTHORISED** | Isolated new version and explicit user approval |

## Acceptance process
- **Technical PASS** requires a named criterion, test or file comparison, actual execution and retained evidence. Static existence does not prove usable functionality.
- **Human PASS** is only granted by the owner for musical quality, UX, major design and release suitability. Do not infer it from automation, older unrelated approvals or lack of complaints.
- **Release/PROMOTION** is a separate explicit decision. A passing prototype is not an automatic published release.
- **Failed/blocked/not attempted** tasks remain visible with exact reasons; never blend those categories into a favourable percentage.
- Every acceptance update records date, scope, baseline hash, testing evidence and decision authority. Preserve superseded historical reports without editing their meaning.
