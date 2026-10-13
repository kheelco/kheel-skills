# Reviewing a job map

A review is a pass over an existing map, reported as findings. For a small change, run stage 1 over what changed and
stop. Judge the map as an inventory of functional steps organised by stage, not as a workflow: a step is never a
finding because it does not follow the one before it, or because an occasion of the job does not pass through it.

1. **Structure.** Report each as a count, listing the steps.
   - The map's job is not in the topology, or its executor differs from the topology's.
   - No pre-check recorded: the job not confirmed in the topology before steps were placed.
   - Steps with no stage, or a stage outside the eight; steps with sub-steps; two steps with the same statement.
   - Steps spanning several things with no **Covers**, or with sub-steps where Covers or separate steps were meant.
   - Fewer than about ten steps (stated too broadly) or far more than twenty (job too high), as guidance; systems,
     products or instruments named in step statements.
   - Constituent candidates not classified, or classified without being reported to the topology.
   - Circumstances listed with the map but not tested for coverage; circumstances or edge cases given maps of their own
     instead of being folded into the steps they change.
   - Circumstances recorded as edge cases or the reverse; cases on steps they do not change; cases not written as
     `<case>: <what the step must accomplish>`; edge cases named in words the glossary does not hold; the same case
     named two ways; circumstances not in the map's list; edge cases tried in the topology that no step takes up.
   - Outcomes not in the standard form (direction + measure + object + clarifier).
   - In a synced map: entries whose YAML block lacks `id`, `version` or `lastUpdated` (other than steps not yet
     pushed); two entries with the same `id`.
2. **Functional coverage and placement.** Has the map found the work the job needs, and is each step where its
   function puts it?
   - **Coverage across circumstances**: for each circumstance and significant edge case, work the job needs there that
     no step holds; boundaries left ambiguous; circumstances that may be other jobs, not reported to the topology.
   - **Placement**: steps placed by when they happen, what they are called or a resemblance to the stage, rather than
     their functional purpose; Conclude used for *what happens when the object ends* where that is not part of this job;
     ambiguous placements forced without the competing readings recorded. Ordinary placements need no justification.
   - **Flow reasoning**: a map criticised, or split, because its steps do not form one sequence; work made a separate
     job or map because it has its own sequence, trigger, source, completion or success criterion.
   - **Constituents**: a candidate forced to covered or to separately mappable where both hold; separate mappability
     claimed without a distinct functional objective; a separately mappable candidate's map that repeats this map's
     steps; several separately mappable with no granularity check; the map held up for unresolved candidates.
   - Stages filled for their own sake; several thin steps under one stage; steps that read as an operating cycle;
     empty stages with no note of what they suggest about the boundary.
   - Steps naming a system, document, screen or hand-off; steps whose verb belongs to a system rather than the
     executor; steps stated as operations rather than what is accomplished.
   - Steps accomplished by someone other than the executor: stakeholder jobs leaking in. Steps that do a receiving
     job's work past the hand-off; steps that do not serve the job's desired result.
   - Steps that transcribe glossary activities.
   - Checks inside Execute, or commitments inside Confirm.
   - Steps whose execution happens in or arrives from the world, unmarked. Where a seam runs both ways: Confirm steps
     that assume the change has already happened; no test against a case where the entry makes the change.
   - A job statement that assumes whether the change comes before, during or after the job; an assurance job with no
     named standard, or one that compares with sources and claims correctness without testing whether the evidence is
     sufficient.
   - Steps whose outcomes answer different questions (authority and eligibility) with neither split nor grouping.
3. **Outcomes**, reviewed separately: a step is not a finding because its outcomes are incomplete, and a missing
   outcome is not a missing step. Initial maps are not expected to be exhaustive.
   - Wording: outcomes that are not measurable, name a solution or method, leave their object or context vague, or
     duplicate another outcome on the same step.
   - Outcomes that restate their step or contain a target; outcomes that are design requirements; outcomes that measure
     another job's result.
   - Outcomes beyond the executor's reach, or owning the resolution of work handed on; time outcomes with no measure;
     invariants stated as outcomes; effort outcomes that time or likelihood would state more precisely.
   - Qualifiers on the job that yielded no outcome.
   - Where outcomes have been researched with practitioners: significant steps still with none.
4. **Drafts.** Steps or outcomes marked attested with no source. In the agreed map: open questions waiting a long time.
5. **Against the rest**, if the other artefacts are to hand.
   - Nouns in steps and outcomes that the glossary does not hold (vocabulary drift).
   - Scenarios whose case the map cannot account for (the strongest check of coverage); steps no scenario needs.

Report findings, not fixes, and offer fixes as proposals grouped by the change they imply (restate, split or merge,
move to another stage, add a step for a coverage gap, classify a constituent, move out, restate an outcome).
