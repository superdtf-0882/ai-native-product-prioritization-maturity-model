# Changelog — AI-Native Product Prioritization Maturity Model

## v1.1.1 — 2026-07-28

**Bug fix, found while building the Whole-Model View:** each dimension's table header declared six columns (Level, Dimension-specific state, Maturity definition, Indicative evidence, Transition to next level, Verification), but every data row only ever had five cells — "Dimension-specific state" and "Maturity definition" were never two distinct columns; the transcription from the workbook merged them into one cell under the wrong label, and the header was never corrected to match. Fixed by removing the phantom "Dimension-specific state" header — the remaining "Maturity definition" column is exactly the cell that was always there. No description text changed, no maturity content affected; this is a header-label correction only, caught by a hard column-count check while writing a parser against this file.

Also landed `short_form.yml` — a 15-cell, one-sentence-per-level compression for the Whole-Model View, same discipline as the SDLC and PDLC compressions.

## v1.1.0 — 2026-07-28

Added a **Verification** column to each dimension's table — an explicit, practical test of whether a transition (A→B, B→C, C→D, D→E) actually happened, not just claimed, matching the family's own precedent (SDLC's D4–D13, PDLC's D4–D12). 12 new clauses across D1–D3. Level E's own row is unchanged — its existing "Sustain: ..." text already serves this purpose.

No change to any dimension's underlying maturity-state content — the existing "Indicative evidence" and "Transition to next level" columns are unchanged; this adds a missing verification layer only.

## v1.0.0 — 2026-07-28

First locked baseline, repo created. Content transcribed verbatim from `AI_Native_Product_Prioritization_Maturity_Model_v1.0.xlsx` (retained in the `ai-native-sdlc-maturity-model` repo as historical working evidence), which itself received four content fixes on 2026-07-26, prior to this repo's creation:

1. **Vocabulary retrofit** — the stale pre-lock level names corrected to the family's Nascent/Modeled/Continuous/Integral/Telemetric, applied throughout the Maturity Matrix and Reference sheets.
2. **Six literal S0 references removed** from public-facing text (found by a full-workbook grep, not assumed limited to what a review brief happened to name).
3. **A version-convention disambiguation note added** (Read Me, A3): this workbook's own "Version 1.0" is personal file-versioning, independent of the family's separate v0.9/v1.0 governance-lock vocabulary.
4. **The 2015 Strategic Value Matrix attributed to David Facer by name** at its one real citation (D1's Level E definition).

David's own ruling (2026-07-26, `briefs/2026-07-26-prioritization-v1-resolution/`) confirmed the workbook's content stands at v1.0, current — the family vocabulary lock was the one stated condition on an earlier "revert to v0.9" ruling, and that condition is now met.

Repo creation itself was held behind a separate condition — `OI-040`'s sequencing gate on this practice's own SDLC maturity (D6 closing, D4 incrementing) — resolved 2026-07-27.

No content changes at this lock beyond transcription from the workbook to markdown. D1–D3 are this model's own content throughout — unlike the PDLC model, this model does not inherit any dimension from the shared intelligence layer; its three dimensions (Value Model Coherence, Decision Governance & Portfolio Integration, Outcome Calibration & Adaptation) have no SDLC/PDLC equivalent.
