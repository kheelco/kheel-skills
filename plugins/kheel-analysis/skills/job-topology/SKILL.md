---
name: job-topology
description: >-
  Use when working out what jobs make up a domain before any of them is analysed in depth: who the job executors
  are, what the core functional job is, and which adjacent and related jobs surround it (Jobs to be Done,
  Outcome-Driven Innovation). Trigger on "job topology", "who is the job executor", "what's the core functional
  job", "main job", "adjacent jobs", "related jobs", "survey the jobs in this domain", "frame the domain", "what
  jobs are there here", "functional job statement", "Ulwick", "ODI", "are these the same executor", or when a domain
  analysis is starting and nothing has been mapped yet. Also trigger when a job map is growing steps that belong to
  someone else's job.
---

# Job topology

A **job topology** surveys a domain's jobs before any of them is opened up: who is trying to get something done, what
the core job is, and which other jobs sit around it. It is the inventory, sized and bounded, so that the deep work (a
job map) is pointed at the right thing. It is the head of the job family: the jobs it names are what job maps open up
and what scenarios are traced through.

*Job* is meant in the Outcome-Driven Innovation sense (Ulwick): a **functional job** the executor is trying to get
done, stated without reference to any solution, stable across changes in process and technology, and decomposable into
the steps of a job map. It is not a situational need statement (*when… I want to… so I can…*), which records a moment
and a motivation; a functional job records an accomplishment.

A topology describes the domain, not a product. The jobs exist whether or not any system does, and the topology should
read as true for an organisation that does the work on paper.

## Principles

- **The domain, not the system.** Jobs, executors and steps are stated so they survive the system's absence. No
  features, screens, workflows, org structures or mechanisms in a job statement.
- **Written in the glossary's words.** A job is a verb on glossary nouns: *maintain the register of members*. A noun
  the glossary does not hold is either badly chosen or a missing term; send it to the `glossary` skill.
- **Evidence, not inference.** While drafting, mark each job, executor and relation *attested* (a source says so),
  *inferred* (concluded from evidence; say from what) or *proposed* (a modelling choice awaiting agreement). Never
  invent an adjacent or related job to make the survey look complete: a topology with a main job and nothing else is a
  finding (nobody has looked around), not a gap to fill.
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
4. **Settle the executor and the core job** ([jobs](references/jobs.md)): the executor by capacity, the core job as
   verb + object + contextual clarifier, at an altitude that passes the three tests.
5. **Place the other jobs.** For each candidate: a job or a step? If a job, adjacent (same executor) or related
   (another executor), how it stands to the main job, and its core intent and how that differs from the main job's.
   Steps go to the job map, not here.
6. **Frame it.** The core executor and job, execution seams, and any sub-domain split already evident, as a hypothesis.
7. **Check** the structural checks in [review](references/review.md) over what changed and every job that names it, and
   list the open questions.
8. **Propose, agree, then write**, doing the full ripple of any change (below) in the same sitting.
9. **Render or sync** in the shape the reader needs ([format](references/format.md)).

### When to stop

A topology is **provisionally complete** when the main executor and main job are settled, each other job is placed
with its executor and its difference from the main job stated, and every question that could change which job is main,
or whether a candidate is a job or a step, is recorded. Map the main job then; the topology will be revisited as maps
send jobs back.

## Changing a job

| Change | What it touches |
|---|---|
| **Restate** | Its job map's heading and every scenario or artefact that cites it. Keep the old wording in its notes until citations are updated. |
| **Change executor** | Its category (an adjacent whose executor changes becomes related, and the reverse), and every step of its map. |
| **Demote to a step** | It leaves the topology for the map of the job it belongs to; its outcomes go with it. |
| **Promote a step** | A step found to have its own intent, lifecycle or outcome becomes an adjacent or related job, and leaves its map. |
| **Change the main job** | Every other job's category and relation, which are stated against it. Usually means the altitude was wrong; re-test it first. |
| **Retire** | Only when nothing cites it, and its map (if any) is retired with it. |

## Alongside other analysis

- **Glossary.** Every noun in a job statement should be a glossary term, and executors are agent terms. Topology work
  is one of the main ways new terms are found.
- **Job map.** Each job may be opened up with a job map (the `job-map` skill), and the main job usually is. A map that
  grows steps belonging to another executor sends them back here as related jobs.
- **Scenarios.** Scenarios trace concrete cases through jobs and their maps; a scenario that cannot say which job it
  belongs to has found a gap in the topology.
- **Later work.** Executors are where actors begin; execution seams tell product work what can only be received, not
  performed.

## Reference

| File | Holds |
|---|---|
| [references/elicitation.md](references/elicitation.md) | The questions to ask, and harvesting jobs from notes |
| [references/jobs.md](references/jobs.md) | Executors, the core functional job, altitude, adjacent and related jobs, qualifiers and circumstances, framing, errors to watch for |
| [references/review.md](references/review.md) | Reviewing a topology: the checks and reporting |
| [references/format.md](references/format.md) | The topology document, drafts, syncing, rendering and where it lives |

[README.md](README.md) describes the job family and its domain model for people integrating it with other systems; it
is not needed to use the skill.
