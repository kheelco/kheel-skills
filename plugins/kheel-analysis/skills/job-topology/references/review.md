# Reviewing a topology

A review is a pass over an existing topology, reported as findings. For a small change, run stage 1 over what changed
and every job that names it, and stop.

1. **Structure.** Report each as a count, listing the jobs.
   - Not exactly one main job.
   - Jobs with no executor; executors with no job; executors with no stated capacity.
   - Adjacent or constituent jobs whose executor is not the main executor; related jobs whose executor is (misfiled).
   - Related jobs with no relation to the main job, or one outside the listed relations.
   - Jobs other than the main job with no stated intent and difference.
   - Episodes with no trigger.
   - Two jobs with the same name.
   - Job maps whose job is not in the topology.
   - In a synced topology: entries whose YAML block lacks `id`, `version` or `lastUpdated` (other than jobs not yet
     pushed); two entries with the same `id`.
2. **Jobs: the checks that need reading.**
   - Job statements containing a feature, system, document or mechanism, or assuming whether a change comes before,
     during or after the job.
   - The main job failing an altitude test; its object's breadth untested against edge cases.
   - Jobs that change the world filed as the main executor's adjacent jobs, or folded into the main job.
   - Episodes of the main job listed as adjacent jobs; obligations classified as steps or jobs without the outcome
     question answered, or stated as domain rules without the source checked.
   - Adjacent jobs whose scope is wider than the main job's object (a broader job's obligation), or whose statement
     does not match the signal given for them.
   - Episodes at different altitudes: an undertaking with its own beginning and end listed beside routine episodes.
   - Related jobs that do not help establish the main job's boundary; no note of related jobs left out.
   - Executors or jobs merged because they stand to the main job the same way, though their desired outcomes differ.
   - Adjacent jobs justified by trigger, recipient or completion alone, with no distinct desired outcome.
   - Classifications written as domain assertions; claims marked inferred that rest on sources not yet read.
   - Jobs named for an output, conflating a consumer's job with a supplier's.
   - Work the executor does to help another's job recorded as their own job.
   - Two executors whose desired outcomes are the same, split on scale, volume or infrastructure.
   - Executors named by title or office where capacity is meant.
   - Emotional and social qualifiers mislabelled, or with no evidence; emotional or social jobs recorded as jobs;
     consumption-chain or purchase jobs present.
   - Seams stated one way where recording gives the change its effect.
   - Differences that name no signal: a job asserted as distinct without saying how.
   - The three questions (breadth, one job or several, changing against recording) neither settled nor recorded as
     open.
   - In a draft: jobs marked attested with no source; inferred jobs nobody has confirmed. In the agreed topology: open
     questions waiting a long time.
3. **Against the rest**, if the other artefacts are to hand.
   - Nouns in job statements that the glossary does not hold (vocabulary drift); executors that are not agent terms.
   - Jobs mapped against jobs not mapped: where the deep work has and has not gone.
   - Steps in job maps whose executor is not the job's: related jobs leaking into maps.
   - A main job whose map needs several independent cycles: constituent jobs not yet recognised.
   - Scenarios that name no job.

Report findings, not fixes, and offer fixes as proposals grouped by the change they imply (restate, change executor,
demote to a step or episode, promote, episode to constituent job, change the main job, retire).
