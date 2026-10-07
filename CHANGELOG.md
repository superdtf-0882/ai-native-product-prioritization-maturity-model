# Changelog — AI-Native Portfolio Prioritization Maturity Model

## v1.4.0 — 2026-10-07

**Renamed: the AI-Native Portfolio Prioritization Maturity Model**, formerly the AI-Native Product Prioritization Maturity Model. The model always graded prioritization across the whole portfolio, product and internal work alike, scored on one value model as fungible assets; the name now says so, which is truer to its roots.

- The title and the first paragraph.
- The four cells that used the old name: D1's core question ("Is portfolio value explicit…"), D1's definition ("an explicit model of portfolio value"), D1-C ("a shared portfolio-value model") and D3-E ("Portfolio prioritization operates as a continuous learning loop"). One word each; no level's ladder changed.
- A new section, **Roots**, before *The 2015 Strategic Value Matrix*: the method's 2010 origin, in the author's words. The 2015 section is unchanged.
- `README.md` and `strategic_value_matrix.md` use the new name. Earlier entries below keep the name they were written under.

Scores against v1.3.0 remain comparable: no level's substance changed; D1 and D3 now name the portfolio, product and internal work alike, which the model always meant.

The repository and the matrix file keep their names (`ai-native-product-prioritization-maturity-model`, `ai_native_product_prioritization_maturity_model.md`): sites load the model by them, so they are identifiers, and identifiers stay while titles change.

## v1.3.0 — 2026-10-01

Added the **Strategic Value Matrix** as this model's Level E reference pattern — the one the matrix already names, "The 2015 Strategic Value Matrix" — for aimaturitymodels.com's Strategic Value Matrix page, in the same shape as v1.2.0's `deep_dives/`:

- `strategic_value_matrix.md` — the method's frame in public words: the geometric scale, the two composites, dependency lift, the tiebreak, and leaving the ranking at a declared reach. Frame version 1.10.
- `svm_sample.yml` — seven illustrative criteria and eight fictional initiatives, labelled as examples. An adopter's criteria and weights are its own.
- `svm_conformance.yml` — the cases any implementation must pass, including a chain that an implementation following dependencies only part of the way ranks wrongly.

**No change to the matrix itself:** `ai_native_product_prioritization_maturity_model.md` is byte-identical to v1.2.0.

## v1.2.0 — 2026-07-28

Added `deep_dives/` — narrative-style Per-Dimension Deep-Dive essays for all three dimensions (Value Model Coherence, Decision Governance & Portfolio Integration, Outcome Calibration & Adaptation), for aimaturitymodels.com's Deep-Dive pages, matching the SDLC and PDLC models' own precedent. Authored fresh, grounded in this matrix's own v1.1.1 locked content, including the per-transition verification clauses and the corrected column structure. No change to the matrix itself.

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
