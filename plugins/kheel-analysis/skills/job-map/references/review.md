# Reviewing a job map

A review is a pass over an existing map, reported as findings. For a small change, run stage 1 over what changed and
stop.

1. **Structure.** Report each as a count, listing the steps.
   - The map's job is not in the topology, or its executor differs from the topology's.
   - Steps with no type, or a type outside the eight.
   - Steps with sub-steps.
   - No record of the coherence test: the principal progressions not written and compared before steps were typed.
   - A conclusion that the job holds together resting on coverage (every episode found a step) rather than on one
     shared beginning, desired result and completion.
   - For a continuing job: episodes that could each be given a Define-to-Conclude progression of their own, mapped as
     stages; steps falling into independent cycles (constituent jobs not reported to the topology).
   - Two steps with the same statement.
   - Significant steps with no outcomes.
   - Outcomes not in the standard form (direction + measure + object + clarifier).
   - In a synced map: entries whose YAML block lacks `id`, `version` or `lastUpdated` (other than steps not yet
     pushed); two entries with the same `id`.
2. **Steps and outcomes: the checks that need reading.**
   - Steps naming a system, document, screen or hand-off; steps whose verb belongs to a system rather than the
     executor.
   - Steps accomplished by someone other than the executor: related jobs leaking in.
   - Steps that transcribe glossary activities.
   - Types with several thin steps: the map was filled, not found.
   - Steps whose execution happens in or arrives from the world, unmarked.
   - Outcomes that restate their step, name a mechanism, or contain a target; outcomes that are design requirements;
     outcomes that measure another job's result.
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
