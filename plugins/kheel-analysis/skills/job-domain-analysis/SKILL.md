---
name: job-domain-analysis
description: >-
  Use when analysing how a domain's distinct jobs relate to one another, beyond discovering them: whether two
  candidates are one job or two, whether a candidate belongs to the main job or beside it, whether two people are one
  executor; how jobs of different executors change, enable, constrain, govern or consume one another; execution seams,
  including where recording gives a change its effect; event-driven and periodic obligations; and testing boundaries
  against exceptional cases, settings and change. Trigger on "how do these jobs relate", "is this one job or two", "is
  this part of the main job or beside it", "are these the same executor", "job dependencies", "who governs this",
  "execution seam", "does recording make the change", "domain analysis of the jobs", or when a job topology or job map
  leaves a boundary between jobs unresolved. Optional: a job map can be made straight from a job topology. What
  happens inside one job (its steps, episodes and sub-jobs) is the job map's work.
---

# Job domain analysis

A **job domain analysis** examines how the jobs a topology has found relate to one another: their identity where it
is in question, the relationships between them, where their work crosses into the world, the obligations around them,
and whether their boundaries hold. It is an **optional enrichment** of the job topology (the `job-topology` skill),
not a step every analysis must take: the topology is enough to start a job map. Use it when the topology records
boundary questions it could not settle, when a map exposes a problem at the edge of a job, or whenever a richer model
of how the domain's jobs fit together is wanted.

It works **between** jobs. What happens **inside** a job (whether a piece of work is a step, an episode or a sub-job
with its own map) is discovered by the job map, which classifies the topology's constituent candidates.

**It enriches the topology; it does not redefine it.** The topology remains the authoritative inventory of jobs and
executors. This analysis refers to its jobs by name and adds what the topology deliberately leaves out. Where the
analysis concludes that the topology is wrong (two jobs are one, an executor is two), it proposes the change to the
topology, which is made there.

This goes beyond what Outcome-Driven Innovation formalises. Ulwick names core, related and emotional jobs and maps one
job at a time; classifying cross-job relationships, seams and obligations is this family's own extension, consistent
with that framework but not part of it.

## Principles

The family's principles apply: the domain, not the system; written in the glossary's words; evidence (attested,
inferred, proposed) while drafting, with unread sources treated as proposed; draft freely, commit by agreement; rules
of method are not facts about the domain.

- **Classifications are established, not prescribed.** Whether two candidates are one job, or a candidate belongs to
  the main job, is settled by weighing the evidence ([identity](references/identity.md)), and left open where it
  cannot be.
- **No classification for convenience.** A classification chosen because it yields a tidier model or map is a
  defect.

## Workflow

1. **Name the task**: settling the topology's open boundary questions; analysing relationships; checking seams or
   obligations; validating boundaries; reviewing.
2. **Read the topology** for the domain and its open classifications, flagged seams and boundary questions; and any job
   maps already made. If there is no topology, make one first with `job-topology`.
3. **Settle identity between jobs** ([identity](references/identity.md)): for each open boundary question (one job or
   two; part of the main job or beside it; one executor or two), weigh the five tests and propose the change to the
   topology. Leave a job's internal structure to its map.
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
- **Job map**: discovers each job's internal structure (steps, episodes, sub-jobs) and reports it to the topology;
  this analysis reads the maps where it needs that structure, and a map that exposes a problem at the edge of a job
  comes back here.
- **Glossary**: every job and case named here is written in its words; analysis is a source of new terms.

## Reference

| File | Holds |
|---|---|
| [references/identity.md](references/identity.md) | Identity between jobs (one job or two; part of the main job or beside it; one executor or two), boundary validation |
| [references/relationships.md](references/relationships.md) | Kinds of relationship, changing the world against recording it, seams, obligations, supplying another job |
| [references/review.md](references/review.md) | Reviewing an analysis |
| [references/format.md](references/format.md) | The analysis document and where it lives |
