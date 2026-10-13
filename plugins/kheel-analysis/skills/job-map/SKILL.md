---
name: job-map
description: >-
  Use when breaking one functional job down into the steps its executor must accomplish and, for each step, the
  desired outcomes by which they judge it done well (Jobs to be Done, Outcome-Driven Innovation). Trigger on "job
  map", "map the job", "job steps", "desired outcomes", "outcome statements", "ODI outcomes", "minimise the time it
  takes to", "minimise the likelihood that", "define locate prepare confirm execute monitor modify conclude", "what
  does the executor have to accomplish", or when a job from a job topology is ready to be opened up. Also trigger when
  a process map, user journey or workflow is being offered as a job map.
---

# Job map

A **job map** is a structured inventory of the **functional steps** required to get one job done, organised by
Ulwick's eight stages, with each step's **desired outcomes**: the measurable qualities by which the executor judges
that step done well. It is not an execution workflow. Its **completeness** is judged by whether it covers the job
across the circumstances it is done in; its **coherence** by whether each step makes a functional contribution to the
job and sits in the stage that contribution belongs to. Neither depends on the steps forming a single sequence.

A job map is not a user journey, a software workflow, a process map of the current organisation, a sequence of screens
or a description of an existing solution. Execution may happen partly or wholly outside any system, and the map must
read as true either way.

The job comes from the **job topology** (the `job-topology` skill): the survey of a domain's jobs, each with its
executor. Map a job from the topology; where there is none, state the job and executor at the top of the map in the
topology's form (verb + object + contextual clarifier; executor by capacity) and resist mapping a job that turns out to
be a step of a larger one.

## Principles

- **The domain, not the system.** Steps say what the executor must accomplish, not how today's process or software
  makes them do it.
- **Function, not flow.** Steps sit under a stage for what they contribute, not for when they happen. A step need not
  follow the one before it, an occasion of the job need not pass through every stage, and work with its own sequence
  is not, for that reason, a separate job ([steps](references/steps.md), *What a job map is*).
- **Written in the glossary's words.** A step is a verb on glossary nouns. Mapping is one of the main ways new terms are
  found: a step that cannot be stated cleanly is usually missing a word, which goes to the `glossary` skill.
- **Found, not filled.** The eight stages are questions to ask, not slots to fill. A map with six steps that were
  found is better than one with eight where two were invented.
- **Evidence, not inference.** While drafting, mark each step and outcome *attested*, *inferred* (say from what) or
  *proposed*. Outcomes harvested from complaints are the executor's; outcomes the agent reasons its way to are inferred.
  A source cited but not read supports nothing yet: a claim resting on one is *proposed*, noted as unverified with its
  citation, until the source is checked.
- **Draft freely; commit by agreement.** Changes to an agreed map are proposed, with why, and written once the user
  agrees. Agreement settles what the map says, not what the evidence establishes: material doubt stays in notes.

## Workflow

1. **Name the task.** A question about a step or outcome; mapping a job; harvesting from notes; changing a map;
   reviewing; rendering or syncing.
2. **Pre-check** ([steps](references/steps.md), *Pre-check*). Confirm the job and executor from the topology; if
   either is unsettled, settle it first (with the `job-topology` skill): a map of the wrong job is worthless however
   good. Take in the main job's constituent candidates, and its circumstances and edge cases. Keep the job statement
   neutral about whether the change it concerns comes before, during or after it, and for anything that gives
   assurance, confirm its standard. **By default, map the job over its life**: one map, with circumstances and edge
   cases folded into the steps they change.
3. **Find the steps.** Work the eight stages as questions about the job, writing down only what is found
   ([elicitation](references/elicitation.md)). Add a step only where it is an accomplishment the job needs in some
   circumstance, never to fill a stage, typically ten to twenty in all; stop at any hand-off to another executor.
   Where a stage yields nothing, ask what that says about the boundary.
4. **Place each step by its function** ([steps](references/steps.md), *Placing a step in a stage*): the stage its
   contribution belongs to, not when it happens or what it is called. Where placement is ambiguous, record the
   competing readings rather than forcing one.
5. **State each step as a milestone**: what the executor has accomplished once it is done, verb + object, in the
   executor's words, no mechanism. A step that a different method would remove without losing an accomplishment the
   job needs is a means, not a step: drop it and move its outcomes to the steps it serves. Mark its execution seam, if it has one.
6. **Classify constituents as they surface** ([steps](references/steps.md), *Constituents, and jobs found while
   mapping*): **covered** (by which steps), **separately mappable**, **outside scope** or **unresolved**; covered and
   separately mappable may both hold. Judge separate mappability by objective, never by a sequence of its own. Do not
   hold the map up for them; report each to the topology. Judge the focal job's granularity by its objective, never by how many
   steps separately mappable candidates cover.
7. **Test coverage across circumstances** ([steps](references/steps.md), *Coverage across circumstances*): for each
   circumstance and significant edge case, does the map contain the functional work needed? Record gaps, ambiguous
   boundaries and circumstances that may be other jobs. Do not draw a workflow for each.
8. **Find each step's outcomes**: how the executor knows it went well, and what takes too long, goes wrong or varies
   ([outcomes](references/outcomes.md)). Check the wording, and that each measures this job's success, within the
   executor's capacity and consistent with the domain's causal rules (who decides, what makes a change take effect). Turn the job's emotional and social qualifiers into outcomes on the steps they bear on. Record
   what the evidence offers; outcome discovery is refined with practitioners, and is not required to be exhaustive now.
9. **Check** the checks in [review](references/review.md) over what changed, and list open questions.
10. **Propose, agree, then write**, then **render or sync** ([format](references/format.md)).

### When to stop

A map is **provisionally complete** when the job is confirmed, every stage has been asked about, each step found is
stated as a milestone with its stage and seam, coverage has been tested against each circumstance, the constituents
have been classified and reported to the topology (unresolved ones included), and the questions that could change a
step's scope or the job's altitude are recorded. Outcomes are recorded where evidence offers them; their completeness
is judged separately, with practitioners. Opportunity scoring is not part of mapping (see
[outcomes](references/outcomes.md)).

## Changing a map

| Change | What it touches |
|---|---|
| **Restate a step** | Its outcomes, which may no longer fit; scenarios that walk through it. |
| **Split or merge steps** | Their outcomes, redistributed one by one, not pooled. |
| **Move a step to another stage** | Its outcomes usually stay; record the competing reading if placement was ambiguous. |
| **Classify a constituent** | Covered (by which steps), separately mappable, outside scope or unresolved, reported to the topology. Mapping a separately mappable candidate makes a new map at a finer level; this map keeps its own steps and outcomes. |
| **Add a step for a coverage gap** | A circumstance whose work the map lacked: add the step, with the case on it, and its outcomes where known. |
| **Move a step out** | A step that pursues a different ultimate result becomes a related job in the topology; a step belonging to another executor becomes a stakeholder job. Its outcomes go with it. |
| **Restate an outcome** | Keep its direction, measure and object in the standard form; a survey already run against the old wording is no longer comparable. |
| **Re-state the job** | The map's heading and the topology entry, together. |

## Alongside other analysis

- **Job topology.** A map opens up one job; steps that are really jobs go back there. The map classifies the
  topology's constituent candidates and reports each back; topology and map refine each other.
- **Job domain analysis** (optional). How distinct jobs relate to one another; a map that exposes an unsettled boundary
  between jobs sends it there.
- **Glossary.** Steps are verbs on glossary nouns. A step is not a glossary activity: an *Audit* the domain names is a
  term; a step is a milestone in getting this job done. One step may involve several named activities, and one may
  recur across steps and jobs.
- **Scenarios.** Concrete cases tested against the map are the strongest test that it covers the job.
- **Later work.** Outcomes are what a product's capabilities are later answerable to, but they are not requirements and
  are not written as though they were.

## Reference

| File | Holds |
|---|---|
| [references/elicitation.md](references/elicitation.md) | The questions to ask, and harvesting steps and outcomes from notes |
| [references/steps.md](references/steps.md) | What a job map is, the eight stages, placing a step, finding steps, the pre-check, constituents and the granularity check, step rules, circumstances and edge cases, coverage, seams, assurance, and errors to watch for |
| [references/outcomes.md](references/outcomes.md) | The outcome statement, the two kinds of completeness, what an outcome is not, checking outcomes, qualifiers, and the opportunity survey |
| [references/review.md](references/review.md) | Reviewing a map: the checks and reporting |
| [references/format.md](references/format.md) | The job map document, drafts, syncing, rendering and where it lives |

The job family and its domain model are described in the `job-help` skill's [README](../job-help/README.md).
