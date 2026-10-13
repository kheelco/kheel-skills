# Reviewing a topology

A review is a pass over an existing topology, reported as findings. For a small change, run stage 1 over what changed
and every job that names it, and stop.

1. **Structure.** Report each as a count, listing the jobs.
   - Not exactly one main job.
   - Jobs with no executor; executors with no job; executors with no stated capacity.
   - Adjacent jobs whose executor is not the main executor; related jobs whose executor is (misfiled).
   - Adjacent or related jobs with no statement of how they stand to the main job, or no stated intent and difference.
   - Two jobs with the same name.
   - Job maps or analyses whose job is not in the topology.
   - In a synced topology: entries whose YAML block lacks `id`, `version` or `lastUpdated` (other than jobs not yet
     pushed); two entries with the same `id`.
2. **Jobs: the checks that need reading.**
   - Job statements containing a feature, system, document or mechanism, or assuming whether a change comes before,
     during or after the job; assurance jobs (verify, check, reconcile) that name no standard.
   - The main job failing an altitude test; its object's breadth untested against edge cases.
   - **Classifications not tested**: candidates classified without weighing the five tests, or on one test alone (a
     trigger and completion, the same executor, a shared higher objective); proposed classifications with no stated
     reasons or uncertainty; candidates left open where the tests clearly point one way, or forced where they split.
   - Jobs that change the world folded into the job that records it, with no flag.
   - Related jobs that do not help establish the main job's boundary; no note of related jobs left out.
   - Executors or jobs merged because they stand to the main job the same way, though their desired outcomes differ.
   - Adjacent jobs justified by trigger, recipient or completion alone, with no distinct desired outcome.
   - Jobs named for an output, conflating a consumer's job with a supplier's.
   - Work the executor does to help another's job recorded as their own job.
   - Two executors whose desired outcomes are the same, split on scale, volume or infrastructure.
   - Executors named by title or office where capacity is meant.
   - Emotional and social qualifiers mislabelled, or with no evidence; emotional or social jobs recorded as jobs;
     consumption-chain or purchase jobs present.
   - Differences that name no signal: a job asserted as distinct without saying how.
   - Classifications written as domain assertions; claims marked inferred that rest on sources not yet read.
   - **Analysis beyond the need**: a topology grown into a full model of the domain's work (systematic relationship
     classification, decomposition of every episode) that belongs to job domain analysis.
   - In a draft: jobs marked attested with no source; inferred jobs nobody has confirmed. In the agreed topology: open
     questions and open classifications waiting a long time.
3. **Against the rest**, if the other artefacts are to hand.
   - Nouns in job statements that the glossary does not hold (vocabulary drift); executors that are not agent terms.
   - Jobs mapped against jobs not mapped: where the deep work has and has not gone.
   - Steps in job maps whose executor is not the job's: related jobs leaking into maps.
   - Topology changes proposed by a job domain analysis or a job map and not yet taken up.
   - Scenarios that name no job.

Report findings, not fixes, and offer fixes as proposals grouped by the change they imply (restate, change executor,
demote to a step or episode, promote, settle an open classification, change the main job, retire).
