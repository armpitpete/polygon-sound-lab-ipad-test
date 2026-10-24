# Project Execution Contract

**Adopted:** 24 October 2026 at the user's explicit request to lock in the agreed execution rules.  
**Scope:** This repository, and a reusable operating contract for Polygon SEQ work. Applying these rules to another repository requires that repository's own state/acceptance records to be consulted; this document does not alter other repositories automatically.

## Mission and responsibility
The project owner defines outcomes, priorities, musical judgements and release approval. The assistant/agent is responsible for discovering existing resources, performing authorised work, testing, preserving evidence, recording progress and following through. Do not shift investigation or routine tool use to the owner. Do not ask the owner to repeat decisions already in the project records.

## Required execution cycle — for every task
1. **Discover first.** Read `PROJECT_STATE.md`, `AGENTS.md`, `TASK_LEDGER.md`, `ACCEPTANCE.md`, the README, relevant commits/issues and connected/local project files. Search all known project repositories **before** declaring a source missing or rebuilding accepted features.
2. **Define the acceptance condition.** Record the expected observable behaviour or immutable artifact, the tests required, and the boundary (including accepted/frozen code).
3. **Execute the authorised work.** Prefer implementation over another list, plan or recommendation. Continue through unblocked work without repeatedly asking for permission. Make nontrivial experiments in isolated versions; do not overwrite frozen versions.
4. **Test on the real target.** For Polygon work: Windows PC first; iPad second. Browser automation is technical evidence, not human user acceptance. Audio hashes do not replace listening.
5. **Independently verify.** Re-read changed files, Git commits, content hashes, build/output artifacts, actual application behaviour and failed tests. Do not equate an attempted operation with success.
6. **Record and continue.** Update a task's status, reason, artifact/evidence link, and outstanding dependency. Then proceed to the next feasible task.

## Exact status definitions
- `PASS`: the specific task's acceptance criterion was met, verified, and has reproducible evidence; documentation alone is not a PASS for an implementation task.
- `FAIL`: an attempted test or operation did not satisfy the criterion. Include error, cause if known, and next corrective operation.
- `BLOCKED`: a required permission, missing dependency, external facility or explicit user decision prevents execution. State exactly which one and what was already attempted.
- `NOT ATTEMPTED`: no substantive task execution occurred. Never disguise this as FAIL or PASS.
- `IN PROGRESS`: actual work performed but the acceptance gate remains open; provide precise interim evidence.
- `DEFERRED`: deliberately scheduled later, with reason and dependency.
Tasks must not be silently omitted. Keep stable IDs. When reporting a total, reconcile the number of PASS, FAIL, BLOCKED, NOT ATTEMPTED, IN PROGRESS and DEFERRED with the entire backlog; never call every listed task 'completed'.

## Before saying "missing" or "blocked"
Check known repos, Git branches/history, existing acceptance files, linked project files, connected PC storage and available archives. A resource register must distinguish:
- `Polygon Sound Lab`: https://github.com/armpitpete/polygon-sound-lab-ipad-test (accepted standalone v0.1.7)
- `Polygon melodic experiment`: https://github.com/armpitpete/polygon-melodic-ipad-test (separate experiment; verify its own state before changing)
- `Polygon SEQ core`: recovered v4.8.6 and later versions in the local Polygon SEQ recovery workspace; **do not assume** a remote repository exists or that a separate experiment is the core repository.

Record the source location and immutable hash when recovered. Search GitHub **before** looking for source replacements. Do not infer acceptance from filenames or generated previews.

## Change boundaries and release control
- Frozen Sound Lab v0.1.7 SHA-256 `087fe68aa84bf569f60d2a158171b4acc3185d555d94c862fcc0b07d3ba43b63` stays unchanged unless the owner expressly approves a new version.
- Preserve the accepted 24 sounds, their presets and the strongly dirty Noise Texture. No silent DSP redesign or sound regeneration.
- Sound Lab Windows acceptance is recorded in `SOUND-LAB-v0.1.7-FINAL-ACCEPTANCE.md`. It **does not** approve Polygon SEQ v4.8.6 integration or later four-workspace designs.
- Preserve accepted Polygon percussion mechanics; new melodic/phase functionality is additive and isolated.
- No Live performance engine work without its separate approval.
- Obtain owner approval for irreversible actions, major architectural changes, release/promotion decisions and human musical/visual acceptance. Do not request approval for ordinary read-only investigation, test execution or already authorised reversible documentation/engineering.
- Never overwrite originals to make evidence appear to match a desired result.

## Reporting
Every meaningful handoff states: exactly what changed, where it changed (path/commit), how it was tested, pass/fail details, what did not run, and the next executable operation. Distinguish *source recovery*, *technical test success*, *human acceptance* and *released product*. Avoid unsupported aggregate success claims, invented acceptance, and open-ended offers to do work that was already authorised.

## Continuity and limits
This repo is the durable record. Conversational memory alone is not a reliable technical ledger; read these files in new sessions. Execution only continues when an authorised tool/workflow is active; do not promise unattended work without a scheduled/persistent mechanism. Where tool access is unavailable, state that limitation without transferring routine diagnostics to the owner.
