# The Strategic Value Matrix

Frame version: 1.10

*Authored by David Facer in 2015, and the reference pattern for Level E Value Model Coherence in the [AI-Native Product Prioritization Maturity Model](ai_native_product_prioritization_maturity_model.md). Derived content, not independently versioned.*

## What it is

A method for ranking work by value against ease, so that a portfolio's competing items can be ordered on one explicit scale. Every item is scored in two halves: what it is worth (**Business Value**) and how readily it can be done (**Ease of Implementation**). The ranking is computed from the scores; nothing about the order is typed in by hand.

This page states the **frame**: the rules every adopter shares. The **criteria and their weights are not part of it**. Each organization sets its own (rule 2). The sample in `svm_sample.yml` uses seven illustrative criteria and eight fictional initiatives so the method can be seen working. **They are examples, not a recommended set.**

## The rules

1. **The scale is geometric, and its ratios are asserted.** A score takes one of four values: Low 1, Medium 3, High 9, Massive 27. Each is three times the last. That is a claim: Massive is worth twenty-seven times Low. **Making the claim is what makes it legitimate to weight and add scores at all.** A 1-to-4 scale only puts things in order; it asserts no ratio between them, so its scores cannot honestly be summed. The ease criteria are scored inverted: a huge item scores 1 and a tiny one 27, so a higher score is always better.

2. **Two composites, with weights summing to 1.00.** Business Value and Ease of Implementation are each a weighted sum of the organization's own criteria, and an item's total is their sum. **The criteria and the weights must be the adopter's own.** So must the split between the two halves, which records how much ease matters against value.

3. **Dependency lift.** If an item ranks below something that depends on it, it inherits that dependent's score: it must be done first, so it ranks as high as the work it unblocks. **The lift runs through whole chains.** A prerequisite of a prerequisite rises too, as far as the chain goes.

4. **Several dependents: take the higher, never the sum.** Summing would count the same value twice, and would put any universal prerequisite permanently at the top.

5. **Ties break toward smaller and safer.** Among equal totals, the item with the higher size inversion plus risk inversion goes first: the smaller, lower-risk item.

6. **A lifted score needs a note.** Any item ranked above its own merit because of a dependency must say why. An unexplained lift is flagged when it occurs, not when someone remembers to look.

7. **Lifted scores are computed, never typed.** Dependencies are recorded; the inherited score is derived from them every time the ranking is computed. **An item's own scores are never adjusted to move it in the ranking.** The lift exists so that adjustment is never necessary.

8. **A prerequisite sorts before its dependent.** Rule 3 makes ties the normal outcome, because a lifted item equals the item it unblocks, and rule 5 knows nothing about direction. **So direction is applied first:** within a tie, prerequisites come before what depends on them, and size and risk decide only what direction leaves open.

## Leaving the ranking

**An item leaves when it is confirmed complete at the reach it declared when it entered**, not when someone marks it done. For public work, the reach is normally the live page a reader actually arrives at. *Done* names a state; a **reach** names where the result can be seen, and the confirmation names how it was checked. **An item finished somewhere nobody looks is still in the ranking.**

## The sample, and the test

- **`svm_sample.yml`** holds seven illustrative criteria, four for value and three for ease, and eight fictional initiatives. Two of the initiatives are prerequisites of others.
- **`svm_conformance.yml`** holds the cases any implementation of these rules must pass. They include a chain of four, which an implementation that follows dependencies only part of the way will rank wrongly, and the cases say so. **A calculator that disagrees with them is not this method.**
