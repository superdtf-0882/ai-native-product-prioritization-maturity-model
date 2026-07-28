# AI-Native Product Prioritization Maturity Model — Matrix

**Version 1.0.0 — 2026-07-28** (first locked baseline. Content originates from David Facer's own working draft, filed as `AI_Native_Product_Prioritization_Maturity_Model_v1.0.xlsx` in the SDLC repo pending the family-wide level vocabulary lock. That vocabulary retrofit, a version-convention disambiguation note, six removed literal S0 references, and the 2015 Strategic Value Matrix's attribution were all landed directly in the workbook (2026-07-26) — see `CHANGELOG.md`. No further content changes at this lock beyond transcription to markdown.)

This model appraises an organization's product prioritization capability — not the elegance of a single scorecard or roadmap decision. It has three dimensions, each independently scored on the same family-wide five-level ladder (A–E) as every other model in this family, but each dimension's own state descriptions, evidence, and transitions are specific to prioritization — they are not shared with or inherited from the SDLC or PDLC models, whose own D1–D3 cover market/persona/positioning intelligence, a genuinely different capability.

**This markdown document is the source of truth.** `AI_Native_Product_Prioritization_Maturity_Model_v1.0.xlsx`, retained in the SDLC repo, is the historical working draft this document was transcribed from — not a distribution rendering of it.

## Purpose

Level A is the least mature state; Level E is the most mature. Each step describes a realistically adjacent operating state specific to the dimension.

## AI-native design rule

AI use does not increase maturity by itself. It increases maturity only when it improves evidence quality, decision coherence, traceability, calibration, or adaptation without obscuring authority or converting inference into fact. The model therefore moves from incidental AI use, to governed participation, to independent challenge, and finally to closed-loop learning.

## The three dimensions

| ID | Dimension | Core question |
|---|---|---|
| D1 | Value Model Coherence | Is product value explicit, multi-dimensional, defensible, and usable by governed human and AI participants? |
| D2 | Decision Governance & Portfolio Integration | Do those value judgments govern real funding, capacity, sequencing, and trade-offs, with explicit human and AI authority? |
| D3 | Outcome Calibration & Adaptation | Does realized evidence improve forecasts, the value model, portfolio decisions, and — when warranted — the originating intent? |

### Maturity-level names

The five letters A–E carry a family-wide name, identical across every dimension and every model in this family (SDLC, PDLC, and Prioritization):

| Letter | Name |
|---|---|
| A | **Nascent** |
| B | **Modeled** |
| C | **Continuous** |
| D | **Integral** |
| E | **Telemetric** |

## The governing loop

Enterprise intent → D1 value model → D2 portfolio decision → execution and outcomes → D3 calibration → portfolio/model correction → reconsideration of enterprise intent when the evidence indicates possible intent failure.

D3-E is the capstone: it distinguishes execution failure, forecasting error, model error, and possible intent failure, then routes each to its proper authority.

| Failure class | What failed? | Primary correction | AI-native contribution | Authority |
|---|---|---|---|---|
| Execution failure | The work did not realize an otherwise sound hypothesis. | Correct delivery, sequencing, capability, or implementation. | Detect variance and assemble evidence without rewriting the original hypothesis. | Delivery / portfolio authority |
| Forecast error | The value, effort, timing, or risk estimate was wrong. | Calibrate scoring anchors, confidence, and forecasting method. | Identify systematic bias by criterion, team, product area, or investment type. | Model owner / portfolio governance |
| Model error | The prioritization model omitted, duplicated, or misweighted a material factor. | Revise criteria, weights, evidence standards, or governance. | Detect model drift and propose explainable changes with preserved provenance. | Value-model authority |
| Possible intent failure | The decision and model may be working against stale, incoherent, or incorrect enterprise intent. | Reconsider originating intent through its proper constitutional authority. | Surface the pattern and evidence; never silently redefine intent. | Enterprise intent authority |

AI does not own the loop. It keeps the evidence, alternatives, consequences, and learning continuously available and governable. Human authority remains explicit at every correction point, especially when the evidence reaches back to the organization's originating intent.

## The 2015 Strategic Value Matrix

Authored by David Facer, predating this model by over a decade, the Strategic Value Matrix is the reference pattern for Level E Value Model Coherence: explicit multi-factor value logic, visible weights, and explainable trade-offs. Overall Level E still requires comparable maturity in decision governance and closed-loop intent calibration.

## How to read this matrix

Each dimension below has a definition followed by a five-level maturity ladder (A through E). A given level is not inherently good or bad; score the normal operating capability — not the best team, workshop, artifact, or AI demonstration.

Dimensions are independently scored — an organization can be advanced in one dimension and nascent in another. Treat the three-grade profile as authoritative; the overall grade is only a directional summary. Prefer proximate improvement: use the current level's transition statement as the next design target, not a longer-range one.

---

### D1. Value Model Coherence

**Definition:** The capability to define and maintain an explicit model of product value that makes unlike drivers comparable without collapsing them — including strategic, customer, market, economic, architectural, delivery, risk, and debt considerations. AI becomes relevant only when it can use, challenge, or help improve that governed model.

| Level | Dimension-specific state | Maturity definition | Indicative evidence | Transition to next level |
|-------|-------------|--------------------------|--------------------------|--------------------------|
| A - Nascent | Priority is determined mainly by advocacy, urgency, executive request, anecdote, or estimated effort. Individuals may use AI privately to draft business cases or make a preferred item sound more compelling, but there is no stable value model against which the output can be tested. | Roadmaps built from requests; inconsistent rationale; private AI-generated business cases; value and effort discussed as one undifferentiated judgment. | Name a small common set of criteria, separate value from implementation difficulty, and require the same logic for every candidate. |
| B - Modeled | A common prioritization method is used — such as value-versus-effort, RICE, MoSCoW, or a simple weighted score. AI may summarize proposals, normalize submissions, or collect preliminary evidence, but criteria remain generic, scoring anchors are weak, and humans manually translate AI output into the model. | Reusable scorecard; simple ranking; AI-assisted proposal summaries; shared criteria with limited definitions; workshop-dependent interpretation. | Define dimension-specific criteria and scoring anchors, state the evidence expected for material scores, and preserve source provenance. |
| C - Continuous | The organization uses a shared product-value model with distinct scoring dimensions, defined scales, and explicit separation of business value from implementation difficulty. The model is structured enough that AI can map proposals to criteria, assemble cited evidence, identify missing inputs, and flag inconsistent scoring. Humans retain responsibility for weights and final value judgment. | Defined scales and weights; separate business-value and implementation factors; machine-readable scoring structure; cited evidence; AI-flagged gaps or inconsistencies. | Assign formal ownership, version the model, test criteria for overlap or double-counting, and make assumptions, confidence, and exceptions visible. |
| D - Integral | The value model is formally owned, versioned, and tied to current strategy and portfolio context. AI performs scenario and sensitivity analysis, challenges unsupported assumptions, detects likely double-counting or scoring drift, and explains why rankings change. The model, weights, evidence standards, and decision authority remain human-governed. | Model owner; version history; criterion provenance; AI-supported sensitivity analysis; confidence notes; scoring-drift review; documented exceptions. | Connect the value model to realized outcomes so evidence can recalibrate scoring anchors, weights, and strategic assumptions. |
| E - Telemetric | A multi-factor strategic value system — of the kind represented by the Strategic Value Matrix — balances revenue magnitude and velocity, strategic alignment, market and customer fit, architecture, implementation size, technical-debt reduction, and delivery risk through explicit scales and weights. AI continuously refreshes relevant evidence, detects model or strategy drift, and proposes changes to criteria, anchors, or weights. Every change remains explainable, versioned, and human-authorized, and the organization can reconstruct why one item outranked another at any point in time. | Governed strategic value matrix; transparent positive and negative drivers; continuously refreshed evidence; explainable scenarios; model-drift detection; preserved decision history. | Sustain empirical and strategic integrity: verify that evidence refresh improves the model without allowing automation, recency, or persuasive inference to redefine value silently. |

### D2. Decision Governance & Portfolio Integration

**Definition:** The capability to turn value judgments into transparent, authoritative portfolio choices that account for funding, capacity, dependencies, sequencing, exceptions, and displacement of other work. AI becomes relevant only when its role, evidence obligations, and authority limits are explicit.

| Level | Dimension-specific state | Maturity definition | Indicative evidence | Transition to next level |
|-------|-------------|--------------------------|--------------------------|--------------------------|
| A - Nascent | Prioritization is a series of local decisions made by the loudest stakeholder, highest-ranking executive, or most urgent customer request. AI may be used privately to strengthen advocacy, but its evidence, reasoning, and influence are invisible. There is no stable decision forum, no visible displacement of other work, and little distinction between recommending, approving, and committing. | Unrecorded overrides; backlog churn; private AI-generated narratives; urgent work inserted without explicit trade-off; no portfolio-level decision record. | Create a recurring decision forum and name who proposes, challenges, decides, records, and commits the outcome. |
| B - Modeled | A scorecard or ranking is used in recurring prioritization meetings, and decisions are documented. AI may prepare summaries, compare proposals, expose obvious conflicts, or record rationale, but it has no governed role and lacks complete access to capacity, funding, dependencies, sequencing, and portfolio context. Executives may still override the result without a standard exception path. | Recurring workshop; ranked list; AI-generated meeting preparation; documented decisions; limited constraint analysis; informal overrides. | Define decision rights, an exception path, the portfolio constraints that must be applied, and the specific AI role in evidence assembly and analysis. |
| C - Continuous | Scoring, challenge, approval, exception, and commitment are distinct and traceable. AI roles and limits are explicit: AI assembles evidence, checks candidate completeness, verifies dependencies and capacity constraints, and records provenance; named humans make consequential decisions. Funding, sequencing, risk, and portfolio balance constrain the ranked list, and the result directly governs committed work within a portfolio. | Decision log; named authorities; governed AI role; evidence provenance; capacity plan; dependency view; exception record; roadmap traceability. | Extend the same decision system across Product, Engineering, Architecture, Finance, and go-to-market portfolios, with common scenario semantics. |
| D - Integral | A shared prioritization system operates across functions and product areas. AI traverses product, engineering, architecture, finance, customer, and go-to-market evidence to model displacement and second-order effects. Independent analysis can challenge the originating proposal and show what is delayed, unfunded, or made riskier when one investment advances. Humans govern the scenarios, thresholds, and final commitments. | Cross-portfolio scenarios; integrated funding and capacity views; AI-supported displacement analysis; independent challenge; architecture and dependency impacts. | Reduce the latency between material evidence changes and governed reconsideration while preserving authority, evidence, and exception discipline. |
| E - Telemetric | Prioritization operates as a standing management system rather than an episodic workshop. New demand enters through a known path; comparable evidence is assembled; alternatives are challenged; and capacity, funding, dependencies, sequencing, and portfolio balance are resolved continuously. AI monitors material changes, maintains decision-ready scenarios, and initiates governed reconsideration. Routine low-consequence actions may be delegated within explicit authority, while consequential portfolio choices remain visibly human-owned. | Governed intake-to-commit flow; live portfolio scenarios; event-driven reconsideration; bounded AI authority; rapid but traceable continue, pause, stop, accelerate, and reallocate decisions. | Continuously test whether adaptive speed is preserving strategic coherence and constitutional authority rather than amplifying short-term noise. |

### D3. Outcome Calibration & Adaptation

**Definition:** The capability to compare predicted value, effort, timing, and risk with realized outcomes; distinguish execution, forecast, model, and intent failure; and return the findings to the portfolio, value model, and — when warranted — the originating enterprise intent.

| Level | Dimension-specific state | Maturity definition | Indicative evidence | Transition to next level |
|-------|-------------|--------------------------|--------------------------|--------------------------|
| A - Nascent | Once work is approved, the prioritization decision is rarely revisited. Delivery may be tracked, and AI may summarize results after the fact, but the original value hypothesis, evidence, assumptions, and intended outcome are not preserved well enough to determine whether the decision was right. | Shipped equals successful; no benefits review; no record of original assumptions; post-hoc AI summaries without a comparison baseline. | For every material decision, preserve the expected outcome, measure, owner, review date, underlying value hypothesis, and originating intent. |
| B - Modeled | Major initiatives receive occasional after-action review. AI helps synthesize retrospectives and compare planned versus actual effort, timing, or selected business outcomes, but the analysis is episodic and selective. Lessons usually affect the next project informally rather than changing the prioritization model or portfolio. | Project retrospectives; AI-assisted synthesis; planned-versus-actual delivery review; informal benefits discussion; isolated lessons. | Require consistent outcome hypotheses and scheduled reviews, and link realized evidence back to the original decision rather than only to delivery performance. |
| C - Continuous | Material prioritization decisions carry explicit expected outcomes, measures, timing, ownership, value hypotheses, and originating intent. AI connects the original decision to subsequent customer, market, financial, delivery, architectural, debt, and risk evidence, flags material variance, and keeps verified evidence, reported information, assumptions, and inference visibly distinct. | Benefits register; decision-to-outcome traceability; named outcome owner; AI-assembled evidence package; forecast-versus-actual review; model-change log. | Measure forecast accuracy and recurring bias by criterion, investment type, product area, and decision team, using independent analysis where practical. |
| D - Integral | AI identifies where the organization systematically overstates value, understates effort, misses timing, discounts risk, or misreads evidence. Forecast accuracy and bias are measured by criterion, team, product area, and investment type. Scoring anchors, confidence ranges, weights, and governance practices are adjusted empirically, and continue, expand, pause, or stop decisions occur before all planned investment is consumed. | Bias analysis; criterion calibration; confidence ranges; independent AI review; stage decisions; evidence-based model revisions; preserved decision lineage. | Close the loop to enterprise intent: distinguish execution failure, forecast error, model error, and possible intent failure, then route each to its proper authority. |
| E - Telemetric | Product prioritization operates as a continuous learning loop. Customer, market, financial, delivery, architectural, debt, and risk evidence is traced back to the original value hypothesis and the intent it served. AI assistance detects variance, systematic bias, model drift, and emerging opportunity while work is still underway, distinguishing execution failure from forecasting error, model error, and possible intent failure. The portfolio, prioritization model, and — when warranted — the originating intent can each be reconsidered through their proper authority, without losing decision lineage or converting inference into fact. | Continuous outcome signals; intent-to-decision-to-outcome traceability; failure-class diagnosis; model-drift checks; early continue, pause, stop, or redirect decisions; preserved evidence and authority lineage. | Sustain epistemic and constitutional discipline: ensure the loop can challenge intent without allowing AI inference to silently become enterprise intent. |
