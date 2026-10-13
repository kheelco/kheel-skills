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

A **job map** breaks one functional job into the **steps** its executor must accomplish to get it done, and gives each
step its **desired outcomes**: the measurable qualities by which the executor judges that step done well. It is the
structure of intent for a job: what must be accomplished, in rough order, and what *well* means at each point.

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
- **Written in the glossary's words.** A step is a verb on glossary nouns. Mapping is one of the main ways new terms are
  found: a step that cannot be stated cleanly is usually missing a word, which goes to the `glossary` skill.
- **Found, not filled.** The eight step types are questions to ask, not slots to fill. A map with six steps that were
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
2. **Confirm the job and executor** from the topology. If either is unsettled, settle it first (with the
   `job-topology` skill): a map of the wrong job is worthless however good. Do not use the step types to decide what
   the job is; a tidier sequence is not evidence of the right job.
3. **Pre-check, and resolve constituents** ([steps](references/steps.md), *Pre-check* and *Resolving
   constituents*). Take in the main job's constituent candidates (a related job mapped on its own has none). **By
   default, map the job over its life**: one Ulwick job map, with episodes passing through the stages they need (the
   continuity rule), circumstances and edge cases folded into the steps they change. As the map takes shape, resolve
   each constituent: **absorbed** (an episode or step); **confirmed as a sub-job**, only if it has a coherent
   progression and outcomes of its own (the mappability test; separately completable is not enough, and a different
   success criterion is not a different job); or **deferred**, with the reason, where it is not needed for the purpose
   in hand. If several are confirmed, check whether the focal job is a higher-order
   objective. **Feed every resolution back to the topology.** Keep the job statement neutral about whether the change
   it concerns comes before, during or after it, and for anything that gives assurance, confirm its standard.
4. **Find the steps.** Work the eight step types as questions about the job, in order, writing down only what is
   found ([elicitation](references/elicitation.md)). Add a step only where it is an accomplishment the job needs,
   never to fill a stage, typically ten to twenty in all; stop at any hand-off to another executor. Modify says where
   the work goes next. Where a type yields nothing, ask what that says about the boundary.
5. **State each step as a milestone**: what the executor has accomplished once it is done, verb + object, in the
   executor's words, no mechanism. Mark its execution seam, if it has one.
6. **Find each step's outcomes**: how the executor knows it went well, and what takes too long, goes wrong or varies
   ([outcomes](references/outcomes.md)). Check each one measures this job's success, within the executor's reach,
   rather than specifying a solution or serving another job's result. Turn the job's emotional and social qualifiers into outcomes on the steps they bear
   on.
7. **Read the map back as a story.** If it only makes sense with a screen in mind, it is a workflow. If a step belongs
   to another executor, it goes back to the topology as a stakeholder job.
8. **Check** the structural checks in [review](references/review.md) over what changed, and list open questions.
9. **Propose, agree, then write**, then **render or sync** ([format](references/format.md)).

### When to stop

A map is **provisionally complete** when the job is confirmed, its constituents resolved (or deferred, with why) and reported to the topology, every step type has
been asked about, each step found is stated as a
milestone with its type and seam, each significant step has outcomes, and the questions that could change a step's
scope or the job's altitude are recorded. Opportunity scoring is not part of mapping (see
[outcomes](references/outcomes.md)).

## Changing a map

| Change | What it touches |
|---|---|
| **Restate a step** | Its outcomes, which may no longer fit; scenarios that walk through it. |
| **Split or merge steps** | Their outcomes, redistributed one by one, not pooled. |
| **Confirm a sub-job** | A constituent passes the mappability test: report it to the topology and map it on its own. The sub-job's map owns its steps and outcomes; this map keeps one step pointing to it (*see the map of …*), with no outcomes of its own, so there is one source of truth. |
| **Absorb a constituent** | Record where it went (an episode passing through which steps, or which step) and report it to the topology. |
| **Defer a constituent** | Record why it is not examined now and report it to the topology, where it stays a hypothesis. |
| **Move a step out** | A step that pursues a different ultimate result becomes a related job in the topology; a step belonging to another executor becomes a stakeholder job. Its outcomes go with it. |
| **Restate an outcome** | Keep its direction, measure and object in the standard form; a survey already run against the old wording is no longer comparable. |
| **Re-state the job** | The map's heading and the topology entry, together. |

## Alongside other analysis

- **Job topology.** A map opens up one job; steps that are really jobs go back there.
- **Job topology, again.** The map resolves the topology's constituent candidates and reports each resolution back;
  topology and map refine each other.
- **Job domain analysis** (optional). How distinct jobs relate to one another; a map that exposes an unsettled boundary
  between jobs sends it there.
- **Glossary.** Steps are verbs on glossary nouns. A step is not a glossary activity: an *Audit* the domain names is a
  term; a step is a milestone in getting this job done. One step may involve several named activities, and one may
  recur across steps and jobs.
- **Scenarios.** Concrete cases traced through the steps are the strongest test that the map is real.
- **Later work.** Outcomes are what a product's capabilities are later answerable to, but they are not requirements and
  are not written as though they were.

## Reference

| File | Holds |
|---|---|
| [references/elicitation.md](references/elicitation.md) | The questions to ask, and harvesting steps and outcomes from notes |
| [references/steps.md](references/steps.md) | The pre-check, resolving constituents and the granularity check, the eight step types, step rules, circumstances and edge cases, seams, assurance, and errors to watch for |
| [references/outcomes.md](references/outcomes.md) | The outcome statement, what an outcome is not, qualifiers, and the opportunity survey |
| [references/review.md](references/review.md) | Reviewing a map: the checks and reporting |
| [references/format.md](references/format.md) | The job map document, drafts, syncing, rendering and where it lives |

The job family and its domain model are described in the `job-help` skill's [README](../job-help/README.md).
