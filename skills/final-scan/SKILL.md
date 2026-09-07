---
name: final-scan
description: Runs the pre-submission checks on a finished draft - word counts, citation reconciliation, flag sweep, convention consistency, and quotation integrity. Use when the user says "final check", "I'm nearly done", "check my draft before submission", "is this ready to submit", or produces a complete document.
---

# Final scan

Run every check, then report by section so the user can work through the list.

## Checks

**Word count.** Count the body and the excluded material separately, per the
rule in `00-Admin/project-config.md`. Report both and say whether the body is
inside the limit. Institutions differ on whether headings, footnotes, tables and
the abstract count; if unrecorded, tell the user to confirm.

**Flags.** Search for every bracketed flag. A submission-ready draft has none.
List any survivors with their locations.

**Citations, both ways.** Extract every in-text citation and every reference
list entry. Report:
- in-text citations with no entry (a marker will check these)
- entries never cited (usually a leftover from a cut passage)
- year and suffix mismatches
- secondary citations formatted correctly, with only the consulted source listed

**Quotation integrity.** Every quotation has a locator. Every verbatim run of
source wording is either quoted or genuinely reworded. Flag anything close to
the source without quotation marks.

**Convention consistency.** One name per concept; consistent cross-reference
form; consistent pronoun convention; house rules observed; spelling uniform.

**Structural sanity.** Chapter numbering continuous; cross-references point to
what they claim; the roadmap in the introduction matches the chapters that
exist; promises made in early chapters ("I address this in five") are kept.

**Primary source integrity.** One edition per work throughout; translators
named; locator systems consistent with the field's conventions; archival
references complete.

**Undercooked prose.** Run the checks from the `revoice` skill across any
passage the user has not yet revised.

## Report

Group findings by section, and within each section put anything that changes
meaning first. Distinguish errors from taste. Say what is clean as well as what
is not: the user needs to know where to stop looking.

If the draft is a PDF, report the issues for the user to fix in their editor
rather than attempting to edit the PDF.
