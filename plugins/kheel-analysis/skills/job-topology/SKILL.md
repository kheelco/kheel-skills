---
name: job-topology
description: >-
  Use when working out what jobs make up a domain before any of them is analysed in depth: who the job executors
  are, what the core functional job is, and which adjacent and related jobs surround it (Jobs to be Done,
  Outcome-Driven Innovation). Trigger on "job topology", "who is the job executor", "what's the core functional
  job", "main job", "adjacent jobs", "related jobs", "survey the jobs in this domain", "frame the domain", "what
  jobs are there here", "functional job statement", "Ulwick", "ODI", "are these the same executor", or when a domain
  analysis is starting and nothing has been mapped yet. Also trigger when a job map is growing steps that belong to
  someone else's job. For how jobs decompose, recur and depend on one another, use job-domain-analysis.
---

# Job topology

A **job topology** discovers and bounds a domain's functional jobs before any of them is opened up: who is trying to
get something done, what the focal job is, and which other jobs sit around it. It is a compact inventory, enough to
point a job map at the right job. It is the head of the job family and the authoritative list of its jobs and
executors: job maps open them up, and job domain analysis (optional) examines how they fit together.

This is an **Ulwick-aligned** method for discovering and bounding functional jobs before Outcome-Driven Innovation job
mapping. Ulwick provides the core functional job, the job executor, related jobs and emotional and social jobs; he does
not prescribe a topology artefact, and this one is the family's own, kept deliberately light. Analysing how jobs
decompose, recur and depend on one another goes beyond Ulwick, and is left to the `job-domain-analysis` skill.

*Job* is meant in the Outcome-Driven Innovation sense (Ulwick): a **functional job** the executor is trying to get
done, stated without reference to any solution, stable across changes in process and technology, and decomposable into
the steps of a job map. It is not a situational need statement (*when… I want to… so I can…*), which records a moment
and a motivation; a functional job records an accomplishment.

A topology describes the domain, not a product. The jobs exist whether or not any system does, and the topology should
read as true for an organisation that does the work on paper.

## Principles

- **The domain, not the system.** Jobs, executors and steps are stated so they survive the system's absence. No
  features, screens, workflows, org structures or mechanisms in a job statement.
- **Written in the glossary's words.** A job is a verb on glossary nouns: *maintain the membership roll*. A noun
  the glossary does not hold is either badly chosen or a missing term; send it to the `glossary` skill.
- **Evidence, not inference.** While drafting, mark each job, executor and relation *attested* (a source says so),
  *inferred* (concluded from evidence; say from what) or *proposed* (a modelling choice awaiting agreement). Never
  invent an adjacent or related job to make the survey look complete: a topology with a main job and nothing else is a
  finding (nobody has looked around), not a gap to fill. A source cited but not read (a provision recalled, a document
  not checked) supports nothing yet: a claim resting on one is *proposed*, noted as unverified with its citation, until
  the source is checked. And a classification the skill's tests produce is a proposal about this domain, not a fact
  about it ([jobs](references/jobs.md), *Rules of method are not facts about the domain*).
- **Draft freely; commit by agreement.** Drafts can be written without asking. Changes to the agreed topology are
  proposed in the conversation, with why, and written once the user agrees. Agreement settles what the topology says,
  not what the evidence establishes: material doubt stays in the job's notes as an open question.

## Workflow

1. **Name the task.** Answering a question about a job or executor; surveying a domain from scratch; harvesting from
   notes; adding or changing jobs; reviewing; rendering or syncing. Do only what it needs.
2. **Find what exists.** The topology for this domain, its glossary, and any job maps already made from it (see
   [format](references/format.md), *Where it lives*). If the topology is synced, check the local copy is not behind.
3. **Gather candidates.** Harvest from what is to hand, then ask about the gaps one or two questions at a time
   ([elicitation](references/elicitation.md)).
4. **Settle the executor and the core job** ([jobs](references/jobs.md)): the executor by capacity (the responsibility
   they carry), split only where the desired outcome changes; the core job as verb + object + contextual clarifier, at
   an altitude and breadth that pass the tests, with edge cases tried. If it is a continuing job, note its episodes and
   what sets each off.
5. **Place the other jobs, selectively.** For each candidate: a step, an episode, or a job? If a job: adjacent (same
   executor, a distinct desired outcome) or related (another executor), with how it stands to the main job in words
   and how its intent differs. Name each job from its own executor's side. Include a related job only where it helps
   establish the main job's boundary, and note those left out. Steps go to the job map.
6. **Record what cannot be settled.** Wherever a classification is genuinely uncertain (a job or a step; one job or
   two; part of the main job or beside it), record it as **open**, with the evidence each way, rather than forcing it.
   A shared higher-level objective is evidence that jobs are related, not that they are one.
7. **Frame it.** The core executor and job; flags for deeper analysis (seams, obligations, supplying); any sub-domain
   split already evident; boundary questions left open.
8. **Check** the structural checks in [review](references/review.md) over what changed and every job that names it, and
   list the open questions.
9. **Propose, agree, then write**, doing the full ripple of any change (below) in the same sitting.
10. **Render or sync** in the shape the reader needs ([format](references/format.md)).

### When to stop

Stop when the **main job, its executor and its principal boundaries** are clear enough to support a job map, and every
unresolved classification is recorded as open rather than forced ([jobs](references/jobs.md), *Ready for mapping*). A
small topology is a good topology. Do not use the step types to settle it, and do not build a full model of the
domain's work here: that is job domain analysis, taken up only if wanted.

## Changing a job

| Change | What it touches |
|---|---|
| **Restate** | Its job map's heading and every scenario or artefact that cites it. Keep the old wording in its notes until citations are updated. |
| **Change executor** | Its category (an adjacent whose executor changes becomes related, and the reverse), and every step of its map. |
| **Demote to a step or episode** | It leaves the topology's jobs: a step goes to the map of the job it belongs to, with its outcomes; an episode goes onto the entry of the job it is an occasion of. |
| **Promote a step** | A step found to have its own intent, lifecycle or outcome becomes an adjacent or related job, and leaves its map. |
| **Settle an open classification** | Usually proposed by job domain analysis or a job map: a candidate becomes a job (adjacent, related, or recorded as part of the main job), a step or an episode; maps and analysis that cite it are updated. |
| **Change the main job** | Every other job's category and relation, which are stated against it. Usually means the altitude was wrong; re-test it first. |
| **Retire** | Only when nothing cites it, and its map (if any) is retired with it. |

## Alongside other analysis

- **Glossary.** Every noun in a job statement should be a glossary term, and executors are agent terms. Topology work
  is one of the main ways new terms are found.
- **Job map.** Each job may be opened up with a job map (the `job-map` skill), and the main job usually is. How a job
  is mapped (over its life, or through parts of it) is the job map's choice. A map that grows steps belonging to
  another executor sends them back here as related jobs.
- **Job domain analysis** (optional). The `job-domain-analysis` skill takes up open classifications, decomposes
  continuing jobs, classifies relationships and settles flagged seams and obligations. It proposes changes to the
  topology; the topology stays the authoritative list of jobs.
- **Scenarios.** Scenarios trace concrete cases through jobs and their maps; a scenario that cannot say which job it
  belongs to has found a gap in the topology.
- **Later work.** Executors are where actors begin; execution seams tell product work what can only be received, not
  performed.

## Reference

| File | Holds |
|---|---|
| [references/elicitation.md](references/elicitation.md) | The questions to ask, and harvesting jobs from notes |
| [references/jobs.md](references/jobs.md) | Executors and roles, the core functional job, altitude and breadth, continuing jobs, open classifications, adjacent and related jobs, flags for deeper analysis, qualifiers and circumstances, framing, ready for mapping, errors to watch for |
| [references/review.md](references/review.md) | Reviewing a topology: the checks and reporting |
| [references/format.md](references/format.md) | The topology document, drafts, syncing, rendering and where it lives |

The `job-help` skill's [README](../job-help/README.md) describes the job family and its domain model for people integrating it with other systems; it
is not needed to use the skill.
