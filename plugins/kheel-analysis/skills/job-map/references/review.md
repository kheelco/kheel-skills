# Reviewing a job map

A review is a pass over an existing map, reported as findings. For a small change, run stage 1 over what changed and
stop.

1. **Structure.** Report each as a count, listing the steps.
   - The map's job is not in the topology, or its executor differs from the topology's.
   - Steps with no type, or a type outside the eight.
   - Steps with sub-steps.
   - No pre-check recorded: the job not confirmed in the topology before steps were typed.
   - Constituent candidates neither resolved nor deferred with a reason, or resolved without being reported to the
     topology; sub-jobs confirmed without a progression and outcomes of their own; a sub-job's steps or outcomes
     repeated in the parent's map; several sub-jobs confirmed with no granularity check.
   - A job fragmented into several maps by episode, trigger or source alone; a map whose choice of form was used to
     decide what the jobs are; in a map of a sub-job, steps that leave its one progression.
   - Stages filled for their own sake; steps that read as an operating cycle; circumstances or edge cases given maps of
     their own instead of being folded into the stages.
   - Circumstances recorded as edge cases or the reverse; cases on steps they do not change; cases not written as
     `<case>: <what the step must accomplish>`; edge cases named in words the glossary does not hold; the same case
     named two ways; circumstances not in the map's list; edge cases tried in the topology that no step takes up.
   - Steps spanning several things with no **Covers**, or with sub-steps where Covers or separate steps were meant.
   - Fewer than about ten steps (stated too broadly) or far more than twenty (job too high); checks inside Execute or
     commitments inside Confirm; systems, products or instruments named in step statements.
   - Jobs split by source or trigger alone; a part with a different ultimate result kept in the map instead of
     reported to the topology.
   - Two steps with the same statement.
   - Significant steps with no outcomes.
   - Outcomes not in the standard form (direction + measure + object + clarifier).
   - In a synced map: entries whose YAML block lacks `id`, `version` or `lastUpdated` (other than steps not yet
     pushed); two entries with the same `id`.
2. **Steps and outcomes: the checks that need reading.**
   - Steps naming a system, document, screen or hand-off; steps whose verb belongs to a system rather than the
     executor.
   - Steps accomplished by someone other than the executor: stakeholder jobs leaking in.
   - Steps that transcribe glossary activities.
   - Types with several thin steps: the map was filled, not found.
   - Steps whose execution happens in or arrives from the world, unmarked.
   - Outcomes that restate their step, name a mechanism, or contain a target; outcomes that are design requirements;
     outcomes that measure another job's result.
   - A job statement that assumes whether the change comes before, during or after the job.
   - Monitor or Modify steps that are activities filed under a stage, not what the executor must accomplish there.
   - Modify steps that say nothing of where the work goes next.
   - An assurance job with no named standard, or one that compares with sources and claims correctness without
     testing whether the evidence is sufficient.
   - Separation of jobs justified by the stage test alone, without a distinct desired result and completion.
   - Jobs split, or reclassified, because the instruction or authority comes from a different source, though the
     desired result and completion are the same.
   - Steps that do not advance the job's completion, or that do a receiving job's work past the hand-off.
   - Steps whose outcomes answer different questions (authority and eligibility) with neither split nor grouping.
   - Outcomes beyond the executor's reach, or owning the resolution of work handed on; time outcomes with no measure;
     invariants stated as outcomes; effort outcomes that time or likelihood would state more precisely.
   - Steps stated as operations rather than what is accomplished; types filled by nearest category; empty types with
     no note of what they suggest about the boundary.
   - Where a seam runs both ways: Confirm steps that assume the change has already happened; no test against a case
     where the entry makes the change.
   - Qualifiers on the job that yielded no outcome.
   - In a draft: steps or outcomes marked attested with no source. In the agreed map: open questions waiting a long time.
3. **Against the rest**, if the other artefacts are to hand.
   - Nouns in steps and outcomes that the glossary does not hold (vocabulary drift).
   - Scenarios that cannot be narrated through the map (the strongest check); steps no scenario passes through.

Report findings, not fixes, and offer fixes as proposals grouped by the change they imply (restate, split or merge,
move out, restate an outcome).
