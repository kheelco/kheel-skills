# Reviewing a glossary

A review is a pass over an existing glossary, reported as findings. Run the stages in order, because each stage's
findings change what the next one means. For a small change, run stage 1 over what changed and its neighbourhood
(every entry that names a changed term, and every entry it names) and stop.

1. **Structure: the checks that inventing content cannot satisfy.** Report each as a count, listing the entries.
   - Relations naming a term that does not exist, or whose kind does not fit its ends (*is a type of* between different
     kinds of term; *captures* naming something that is not a characteristic; *identifies*, *captures* or *is derived
     from* on a term that is not a characteristic; a characteristic's bearer recorded as a *refers to*).
   - Characteristics with no bearer.
   - *Captures* that names no moment.
   - *Refers to* with no label, where the association is not self-evident from the two definitions.
   - A synonym that is also another term's preferred word or synonym, unscoped and with no boundary between the two.
   - Synonyms pointing at a term that does not exist; one word as the preferred term of two entries without
     qualification.
   - Absences that name no setting; variation naming a dimension or setting that is not declared.
   - Two rows with the same preferred word; entries with no row; an entry whose summary fields disagree with its row.
   - Rows missing a required field (term, kind, definition; and the bearer of a characteristic).
   - In a synced glossary: terms with no entry; entries whose YAML block lacks `id`, `version` or `lastUpdated` (other
     than new terms not yet pushed); two entries with the same `id`.
2. **Entries: the checks that need reading.**
   - Definitions that name a screen, feature, table or technology.
   - Definitions that are circular or lean on an undefined term.
   - Examples that do not fit their definition (polysemy); pairs of definitions that differ only in wording
     (synonymy).
   - Kinds that look forced, or unsettled; one entry covering both an act and what it produces.
   - Collisions where the narrower sense is not a case of the broader.
   - Variation that changes the meaning at some setting (a split that has not been made); **Must hold** that differs by
     setting.
   - *Is part of* where the other thing is associated with the whole rather than a component of it, and the reverse.
   - Derivations that name only some of their sources.
   - **Must hold** that is really a domain rule or a system constraint; values in rules that vary by setting.
   - Multiplicity in labels that no source stated, or that rests only on the evidence for the relation; the same
     multiplicity stated in a label and again under **Must hold**.
   - Route-specific requirements filed under **Must hold** that are really set by a jurisdiction, entity form or
     instrument.
   - Kinds chosen from a label's wording ("has" taken to mean *is part of*) rather than by the part-or-associated test.
   - Multiplicity the domain never stated, lifecycle, participants or system behaviour written into entries.
   - In a draft: claims marked attested with no source; inferred ones nobody has confirmed; a term whose attested
     definition is being read as vouching for unmarked claims that were in fact inferred.
   - In the agreed glossary: open questions (*Open:* in notes) that have been waiting a long time, and terms with no
     source.
   - Terms with no example.
3. **Boundaries.** Entries with no *not to be confused with*, and of those, the ones with a near neighbour in the
   glossary that should have been named. This is the pass that turns a list back into a map.
4. **The language against the rest**, if the other artefacts are to hand.
   - **Vocabulary drift:** nouns and named acts in use cases, stories, activities, rules or capabilities that the
     glossary does not hold, or holds under another word. The most valuable finding there is: the other artefacts
     have started speaking a language the glossary does not record.
   - Glossary terms nothing cites: possibly fine, possibly a word nobody actually uses.
   - The share of terms that are coined: a high share means the glossary describes a product, not a domain.

Report findings, not fixes. A review that silently repairs what it finds has removed the evidence of what was wrong.
Offer fixes as proposals grouped by the change they imply (rename, redefine, split, merge, retire, or an edit to one
field), and let the user take them. Where a fix is obvious and mechanical, say so, and still ask.

A review of a glossary held elsewhere reviews what was pulled, and says so: it may be behind its source.
