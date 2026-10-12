---
name: glossary
description: >-
  Use when developing or maintaining the glossary of a problem domain (also called its language model,
  conceptual model or vocabulary): harvesting terms from notes or interviews, defining and bounding terms,
  relating them, recording how they vary by jurisdiction or entity form, renaming, splitting, merging or
  retiring terms, reviewing a glossary, deriving diagrams from it, or syncing it to where it is kept. Trigger
  on "glossary", "define our terms", "what do we call this", "what does X mean here", "are these the same
  thing", "is this a type of that", "ubiquitous language", "domain vocabulary", "terminology", "language
  model", "conceptual model", "harvest the terms", "does this vary by jurisdiction", "rename/split/merge this
  term", "review the glossary", "diagram these concepts", or "sync the glossary".
  Also trigger when two artefacts use different words for one thing, or one word for two.
---

# Glossary

A **glossary** establishes what the terms of a domain mean and how those meanings relate, in a form every
stakeholder can read, so that everyone working on the domain shares one understanding of it through its language.
It is the first concept artefact to build and the one the others are written in: a use case, activity or rule that
uses an undefined noun is ambiguous, and nothing downstream repairs that.

A glossary does **not** establish the complete structural, behavioural or representational model of the domain. It
may hold kinds of term, relations, characteristics and definitional rules, but only to the extent that they clarify
meaning. Multiplicity beyond what the domain itself states, lifecycles, full attribute lists, participants in
activities and the rules a system enforces belong to later work (domain modelling, activity mapping, business rules
and constraints).

What it does establish is a **partial concept system**: a connected understanding of the domain's meanings and the
distinctions between them. It develops progressively as terms are elicited and refined, around the clusters the work
needs. Completeness means sufficient clarity for the work at hand, not an exhaustive representation of the domain.

Two tests keep it there:

- **Would a practitioner say it in a meeting?** An entry that needs a diagram to say is not an entry.
- **Does knowing this change how a practitioner understands or distinguishes the terms?** If so, it belongs. If it
  only decides how the terms are represented or managed by a system, it belongs elsewhere.

*Language* here means the domain's own language, not a large language model.

## Principles

- **The domain, not the system.** Terms come from the people who work in the domain and what they write: interviews,
  workshops, regulation, contracts, their forms and spreadsheets. Not from code, schemas or the backlog, which hold
  the solution's vocabulary. A definition must survive the system's absence.
- **Boundaries before definitions.** What a term is confused with, and the line between them, is usually sharper and
  more useful than the definition. An entry that marks its boundaries turns a word list into a map.
- **Evidence, not inference.** Every claim an entry makes (its definition, kind, example, each relation and rule) is
  *attested* (a source or practitioner says so), *inferred* (you concluded it from evidence, and say from what) or
  *proposed* (a modelling choice awaiting agreement). Status is tracked in drafts: a term is marked by its
  definition's status, and any other claim that differs is marked. The agreed glossary carries no status; a claim
  agreed in while still unconfirmed keeps an open question in the term's notes ([terms](references/terms.md),
  *Evidence*). Never mark something attested that no source
  gave you; never fill a gap with invented content. A missing example is a visible gap; a made-up one is a hidden
  error. Be most wary of type and part relations inferred from similar wording: the domain often uses look-alike words
  for unrelated things.
- **Draft freely; commit by agreement.** Provisional entries (forty terms harvested from an interview, a first pass
  over a new area) can be drafted without asking, kept apart from the agreed glossary and marked as a draft. Changes
  to the agreed glossary — adding to it, or renaming, redefining, splitting, merging or retiring what is in it — are
  proposed in the conversation, with why, and written only once the user agrees. A silent edit is the one that gets
  reverted.
- **The glossary is the source.** Diagrams and other renderings are derived from it. A diagram that shows something
  the glossary does not say is a finding about the glossary.

## Workflow

1. **Name the task.** Answering a question about a term; eliciting terms with a practitioner; harvesting from notes;
   adding or changing terms; reviewing; rendering or syncing. Do only what the task needs: a question about one word
   wants an answer in the console, not a pass over the whole method.
2. **Find the glossary and its scope.** Locate the existing glossary (see [format](references/format.md), *Where it
   lives*), and the domain under investigation and its sub-domains. If it is held externally, check whether the local
   copy is behind before editing. If there is none, ask where it should live.
3. **Gather candidates.** Harvest from what is to hand, then ask only about the gaps, one or two questions at a time
   ([elicitation](references/elicitation.md)). Triage: keep terms with a domain-specific meaning and terms that are
   ambiguous; leave ordinary words in their ordinary sense. Before adding, look for the term under another name.
4. **Define and bound each term.** Its word, a one- or two-sentence definition, its kind, what it is
   not to be confused with, and a real example ([terms](references/terms.md)).
5. **Relate it, where that clarifies meaning.** Use the relation kinds in [relations](references/relations.md), each
   with its evidence, and label each in the domain's words: a reading ("an Invoice has at least one Line item") or a
   role ("primary actor"). The kind implies no multiplicity; a label states it only where the domain does.
6. **Rules and variation, where they arise.** Definitional rules go on the term; contextual domain rules are
   referenced; system constraints leave. A term's meaning is the same at every setting; whether it exists, what it
   is called and which rules govern it may vary ([rules and variation](references/rules-and-variation.md)).
7. **Check.** Run the structural checks in [review](references/review.md) over what changed **and its neighbourhood**:
   every entry that names a changed term (in relations, *Of*, synonyms, boundaries, definitions or variation) and every
   entry a changed term names. A rename is checked at every place the old word appeared, not just on the renamed entry.
   List the open questions that could change an entry's meaning.
8. **Propose, agree, then write** to the agreed glossary, doing the full ripple of any change (below) in the same
   sitting. A draft is promoted the same way: the user agrees the entries, which then join the glossary.
9. **Render or sync** in the shape the reader needs ([format](references/format.md)).

### When to stop

An entry is **provisionally complete** when its definition, kind and boundaries are clear enough for
the task in hand, and every unresolved question that could materially change how it is read is recorded in its notes.
Stop there. The glossary is never finished — every later artefact sends words back — and progressive refinement is the
intended way of working, not a failure to finish.

When working through a whole domain, take one area at a time (a sub-domain, or the cluster around one central term)
and bring it to provisional completeness before moving on. Terms in areas not yet done may be named in relations as
placeholders; do not define them from the far side. The count of placeholders measures what is left.

## Changing a term

A change ripples, and the ripple is the work.

| Change | What it touches |
|---|---|
| **Rename** | Every relation, synonym and characteristic that names it, and every downstream artefact that cites it. The old word becomes a synonym so readers and citations arriving with it still land. A synced term keeps its external ID. |
| **Redefine** | Its types, whose meaning narrows from it; its boundaries, which may have moved; its examples, which may no longer fit. |
| **Split** | A polysemy found. Each sense gets its own entry and relations, each qualified if they share the word; every citation of the old word is re-pointed one by one, not in bulk. |
| **Merge** | A synonymy found. One entry survives with the other's words as synonyms, so citations of either still land. |
| **Retire** | Only when nothing cites it; otherwise it is a finding, since something still speaks a word the domain has stopped using. |

Before a rename, split or merge leaves a word as a preferred word or synonym, check that it does not already name
another term ([terms](references/terms.md), *The preferred term*).

A glossary with a renamed base and un-renamed types is worse than one never renamed, because it now looks deliberate.

## Alongside other analysis

The glossary is the language the other analysis is written in. When an artefact and the glossary disagree about a
word, one of them is corrected deliberately, and never neither. Expect the other work to send terms back:

- **Activity mapping** begins from activity-kind terms and agents, and records who takes part in what; it surfaces the
  objects of verbs.
- **Domain modelling** takes concepts, characteristics and relations as its starting vocabulary and adds what the
  glossary deliberately omits: multiplicity the domain has not stated, lifecycle, full attributes.
- **Use cases and stories** cite glossary terms rather than restating them; agents are where actors begin.
- **Business rules and constraints** receive the contextual rules and system constraints that leave the glossary.

Where those skills are available, hand over to them; where they are not, note what was handed over in the entry's
notes. Comparing the nouns those artefacts use against the glossary (*vocabulary drift*) is the most valuable check
there is ([review](references/review.md)).

## Reference

| File | Holds |
|---|---|
| [references/elicitation.md](references/elicitation.md) | The questions to ask, and harvesting terms from notes and transcripts |
| [references/terms.md](references/terms.md) | Kinds of term, what a term says (summary and entry), evidence, preferred terms, domains and collisions, errors to watch for |
| [references/relations.md](references/relations.md) | The relation kinds, when to record one, and a worked example |
| [references/rules-and-variation.md](references/rules-and-variation.md) | Definitional rules versus domain rules and system constraints; variation across jurisdictions and entity forms |
| [references/review.md](references/review.md) | Reviewing a glossary: the checks, their order, and reporting |
| [references/format.md](references/format.md) | The glossary document (summary table and entries), drafts, syncing, renderings, deriving diagrams, and where it lives |
