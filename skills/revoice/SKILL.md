---
name: revoice
description: Checks the user's own rewritten passages for accuracy damage, dropped qualifiers, misattribution, convention drift and undercooked phrasing, then applies the version they approve. Use when the user submits rewritten prose, says "here's my version", "check this paragraph", "I've rewritten this section", "put this in my words", or is working through a draft chapter by chapter.
---

# Revoice

The user rewrites AI-drafted or source-derived prose into their own voice. This
skill checks what their rewriting broke, without touching what it improved.

Their words are the point. Repair only what is wrong.

## Check every submitted passage on five fronts

**1. Accuracy against the sources and the argument.** The commonest damage,
and the most serious:

- Meaning flips: a missing "not", "un-", or "dis-" that inverts a claim
- Attribution inversions: a view the author attacks described as one they hold
- Dropped qualifiers: "only", "must", "in general", "can", "may" carry logical
  weight; losing one weakens or overstates the claim
- Claims migrating to the wrong source, or the user's own inference presented
  as a cited author's view
- Wrong year, wrong suffix (2024a for 2024b), invented sources

**2. Argument integrity.** Does each step still follow? Watch for fabricated
inferences ("it thus follows" where nothing follows), collapsed contrasts,
premises that now assert what they were meant to prove, and reductios that lost
the absurd conclusion they depend on.

**3. Conventions.** Referencing style, spelling, house rules from
`00-Admin/project-config.md`, terms of art used consistently, cross-reference
form.

**4. Typos and grammar.** Including the ones that change meaning: "nominally"
for "normally", "proscribe" for "prescribe", "enhance" for "deepen".

**5. Undercooked sentences.** Phrasings the reader must reconstruct:

- The wrong subject doing the verb's work ("voluntariness demands more")
- Compressed appositions with the verb elided
- Gnomic three-word closers that assume the reader followed
- Unexplained metaphors and coinages carrying argumentative weight
- Back-pointers with no antecedent: "this account", "the case", "such a choice",
  "their condition" - where the reader must hunt backwards to find the referent
- Vague verbs: "handled", "sits within", "addresses"

## How to report

Number the findings. Put the load-bearing ones first and say plainly which
change meaning. For each, quote the phrase, say what is wrong, and give the
repair.

Then show the full passage with repairs applied, so the user reads it whole.

Then wait. Do not write to the file until the user confirms. A direct
instruction ("fix the typo") authorises that fix and nothing else.

## When the user asks for options

Give three or four genuinely different versions, not synonyms of one. Vary the
structure, not just the vocabulary. Say what each buys and costs: brevity,
emphasis, formality, how much the reader must infer. Recommend one, with a
reason.

## When the user asks what something means

Explain it properly: what the phrase means, what work it does in the argument,
where it recurs, and what an examiner might ask about it. Add the explanation to
`00-Admin/glossary.md`. These questions are the best signal available that a
sentence needs rewriting.

## Never

Do not smuggle in unrequested changes alongside a confirmed edit. Do not restore
material the user has deliberately cut, though you may note once what its loss
costs. Do not smooth their voice towards a house style: register, rhythm and
idiosyncrasy are theirs.
