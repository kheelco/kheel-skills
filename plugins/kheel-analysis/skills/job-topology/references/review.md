# Reviewing a topology

A review is a pass over an existing topology, reported as findings. For a small change, run stage 1 over what changed
and every job that names it, and stop.

1. **Structure.** Report each as a count, listing the jobs.
   - Not exactly one main job.
   - Jobs with no executor; executors with no job.
   - Adjacent jobs whose executor is not the main executor; related jobs whose executor is (misfiled).
   - Adjacent or related jobs with no relation to the main job, or one outside the listed relations.
   - Jobs other than the main job with no stated intent and difference.
   - Two jobs with the same name.
   - Job maps whose job is not in the topology.
   - In a synced topology: entries whose YAML block lacks `id`, `version` or `lastUpdated` (other than jobs not yet
     pushed); two entries with the same `id`.
2. **Jobs: the checks that need reading.**
   - Job statements containing a feature, system, document or mechanism.
   - Main job failing an altitude test.
   - Adjacent jobs with no intent, lifecycle or outcome of their own: steps in disguise.
   - Two executors whose jobs differ only in scale, frequency or seniority: probably one.
   - Executors named by title or department where capacity is meant.
   - Emotional or social jobs recorded as jobs; consumption-chain or purchase jobs present.
   - Differences that name no signal: a job asserted as distinct without saying how.
   - In a draft: jobs marked attested with no source; inferred jobs nobody has confirmed. In the agreed topology: open
     questions waiting a long time.
3. **Against the rest**, if the other artefacts are to hand.
   - Nouns in job statements that the glossary does not hold (vocabulary drift); executors that are not agent terms.
   - Jobs mapped against jobs not mapped: where the deep work has and has not gone.
   - Steps in job maps whose executor is not the job's: related jobs leaking into maps.
   - Scenarios that name no job.

Report findings, not fixes, and offer fixes as proposals grouped by the change they imply (restate, change executor,
demote, promote, change the main job, retire).
