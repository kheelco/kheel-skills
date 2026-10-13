---
name: job-domain-analysis
description: >-
  Use when analysing how a domain's jobs fit together, beyond discovering them: whether candidates are jobs of their
  own, parts of larger jobs (sub-jobs), episodes or steps; how continuing jobs are done through episodes; how jobs of
  different executors change, enable, constrain, govern or consume one another; execution seams, including where
  recording gives a change its effect; event-driven and periodic obligations; and testing boundaries against
  exceptional cases. Trigger on "how do these jobs fit together", "is this one job or several", "is this part of that
  job", "sub-job", "episode", "continuing job", "job dependencies", "who governs this", "execution seam", "does
  recording make the change", "domain analysis of the jobs", or when a job topology or job map leaves a job's identity
  or boundary unresolved. Optional: a job map can be made straight from a job topology.
---

# Job domain analysis

A **job domain analysis** examines how the jobs a topology has found fit together: their identity, decomposition and
episodes, the relationships between them, where their work crosses into the world, and whether their boundaries hold.
It is an **optional enrichment** of the job topology (the `job-topology` skill), not a step every analysis must take:
the topology is enough to start a job map. Use it before mapping when the topology records classifications it could
not settle, after mapping when a map exposes a boundary problem, or whenever a richer model of the domain's work is
wanted.

**It enriches the topology; it does not redefine it.** The topology remains the authoritative inventory of jobs and
executors. This analysis refers to its jobs by name and adds what the topology deliberately leaves out. Where the
analysis concludes that the topology is wrong (a candidate is a job after all, an executor is two), it proposes the
change to the topology, which is made there.

This goes beyond what Outcome-Driven Innovation formalises. Ulwick names core, related and emotional jobs and maps one
job at a time; decomposing jobs, analysing episodes and classifying cross-job relationships is this family's own
extension, consistent with that framework but not part of it.

## Principles

The family's principles apply: the domain, not the system; written in the glossary's words; evidence (attested,
inferred, proposed) while drafting, with unread sources treated as proposed; draft freely, commit by agreement; rules
of method are not facts about the domain.

- **Classifications are established, not prescribed.** Whether something is a job, a sub-job, an episode or a step is
  settled by weighing the evidence ([identity](references/identity.md)), and recorded as undecided where it cannot be.
- **No classification for the sake of a map.** How the jobs will be mapped is the job map's choice, made afterwards; a
  classification chosen because it yields a tidier map is a defect.

## Workflow

1. **Name the task**: settling open classifications from the topology; decomposing a continuing job; analysing
   relationships; checking seams or obligations; validating boundaries; reviewing.
2. **Read the topology** for the domain and its open classifications, flagged seams and boundary questions; and any job
   maps already made. If there is no topology, make one first with `job-topology`.
3. **Settle identity and decomposition** ([identity](references/identity.md)): for each open candidate, weigh the
   identity tests; decompose a continuing job into sub-jobs only where its parts have identity of their own; classify
   its episodes, each with trigger, immediate result and completion.
4. **Analyse relationships, seams and obligations** ([relationships](references/relationships.md)): classify each
   relationship and link it to the most specific job it bears on; separate changing the world from recording it, and
   settle each seam's direction; place each obligation.
5. **Validate the boundaries** against exceptional cases, different settings and change.
6. **Check** the analysis ([review](references/review.md)), and list what goes back to the topology.
7. **Propose, agree, then write** `job-domain-analysis.md` ([format](references/format.md)), and propose the topology
   changes it implies.

### When to stop

When every classification the work in hand depends on is settled or recorded as open with its evidence, the
relationships that shape the main job's boundary are classified, and each flagged seam and obligation is placed. A
domain analysis can be partial: settling one open question is a legitimate piece of work.

## Alongside the other skills

- **Job topology**: the source of the jobs and executors, and the place changes to them are made.
- **Job map**: decides how to map a job, using the decomposition this analysis records (a higher job over its life, or
  its sub-jobs one by one); a map that exposes a boundary problem comes back here.
- **Glossary**: every job, episode and case named here is written in its words; analysis is a source of new terms.

## Reference

| File | Holds |
|---|---|
| [references/identity.md](references/identity.md) | Job identity, decomposition, sub-jobs, continuing jobs and episodes, boundary validation |
| [references/relationships.md](references/relationships.md) | Kinds of relationship, changing the world against recording it, seams, obligations, supplying another job |
| [references/review.md](references/review.md) | Reviewing an analysis |
| [references/format.md](references/format.md) | The analysis document and where it lives |
