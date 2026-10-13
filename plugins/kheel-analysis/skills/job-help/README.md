# The job family

The reference for the job family of skills in this plugin: what each skill does, how the family relates to Ulwick's
Outcome-Driven Innovation, the generic activity model the artefacts are built on (reusable for other kinds of activity
analysis), how that model is configured for Jobs to be Done, and how it maps to and from other systems. It sits with `job-help`, which may
draw on it to answer questions about the model. The skills' own `SKILL.md` files and references remain the authority
on how each artefact is built.

## The family

The family models what people in a domain are trying to get done, at the concept level: describing the domain, not a
product. It is written in the words of the domain's glossary, and is built around Jobs to be Done in the
Outcome-Driven Innovation sense (Ulwick).

| Skill | Primary question | Core unit | Artefact |
|---|---|---|---|
| **job-topology** (the head) | What jobs exist, who does them, and where are their boundaries? | Functional job | `job-topology.md`: a compact inventory of jobs and executors, the main job's constituent candidates, open questions and flags |
| **job-domain-analysis** (optional) | How do distinct jobs relate to one another? | Job, relationship | `job-domain-analysis.md`: identity between jobs, relationships, seams, obligations, boundary tests |
| **job-map** | What must be accomplished to get one job done, and how is each part judged? | Job step | One map per job mapped: an inventory of steps by stage, with desired outcomes; classifies the topology's constituent candidates |
| **job-help** | What is all this, and what do I do next? | None | Explanations, and a guided path through the other skills |
| *scenario* (planned) | Does it hold up against a real case? | Case | Concrete stories traced through a job map |

The three modelling skills are analytical capabilities, not a mandatory sequence. Topology and job map refine each
other: the topology proposes, the map tests and reports back. Job domain analysis can come before mapping, after it, or
when a map exposes a problem at the edge of a job;
`job-help` explains and guides, and makes no artefact of its own.

They sit beside the `glossary` skill:

- jobs and steps are **verbs on glossary nouns** (*maintain the membership roll*), and executors are agent terms;
- the glossary holds the nouns, and only those acts the domain names as things in their own right (*Audit*); the doing
  is modelled here.

What the family shares with the glossary: the domain, not the system; evidence (attested, inferred, proposed) tracked
while drafting and agreement before committing; stopping when it is clear enough for the work at hand; Markdown
documents with a summary table and full entries; no IDs unless synced, and then a YAML block per entry.

Deliberately out of scope, as product-level or heavier than the purpose needs: process flow notations (BPMN), journey
maps and service blueprints, story maps, capability maps, Ulwick's consumption-chain and purchase-decision jobs, and
running opportunity surveys (a map's outcomes are written ready for one).

## Ulwick and the extension

**Ulwick-aligned: job topology and job map.** Together they are an Ulwick-aligned method: the topology discovers and
bounds the functional jobs, their executors and the jobs around them; the job map develops a job into the eight
universal stages (Define, Locate, Prepare, Confirm, Execute, Monitor, Modify, Conclude) and its desired outcomes. By
default a job is mapped **over its life**: for a continuing job, one map holds the steps every episode needs, each episode using only those it needs, and
circumstances and edge cases are folded into the steps they change. This is the path to use for ODI research and
outcome harvesting. Ulwick does not prescribe a topology artefact; the family's topology is its own, kept deliberately
light, and is not offered as canonical Ulwick. *Related job* keeps Ulwick's meaning, the executor's other jobs; the
jobs of other executors that touch the main job are **stakeholder jobs**, the family's own word.

**Topology and map refine each other.** Surveying a domain turns up work that seems to make up the main job (taking in
changes, checking, correcting, setting up). The topology records it as **constituent candidates**, each with what was
noticed and a provisional lean, without deciding what it is. Mapping is where the job's internal structure is
discovered, as in Ulwick's iterative mapping: the job map classifies each candidate as **covered** (its work is
represented by the map's steps), **separately mappable** (a distinct functional objective worth a map of its own, at a
finer level), **outside scope** or **unresolved**, and reports back to the topology. Covered and separately mappable
can both hold, and nothing has to be settled before the map proceeds. The focal job's granularity is judged by the
distinctness and coherence of its objective, never by how many steps separately mappable parts cover; a **higher-order
job**, which the focal job is one means to, is a different objective, noted for the topology.

**A job map is an inventory, not a workflow.** Its steps are organised by the stage their function belongs to, not by
order of execution; one occasion of the job may use only some of them. Its completeness is judged by coverage of the
job across its circumstances, and its coherence by the functional relevance of its steps, not by whether they form a
single sequence.

**The extension: job domain analysis.** Going beyond Ulwick, it examines what lies **between** jobs: whether two
candidates are one job or two, whether a candidate belongs to the main job or beside it, whether two people are one
executor; how jobs of different executors relate; where work crosses into the world; the obligations around them; and
whether the boundaries hold. It **enriches the topology without redefining it**, and leaves what happens inside a job
to the job map.

```mermaid
flowchart LR
    T["Job topology<br/>(discovery; constituent candidates)"] -- "main job" --> M["Job map<br/>(over its life)"]
    M -- "classifications: covered / separately mappable / …" --> T
    M -.-> S["Job map<br/>(a separately mappable sub-job)"]
    T -.-> D["Job domain analysis<br/>(optional; between jobs)"]
    D -. "proposes changes" .-> T
```

Four ideas are kept distinct throughout, and are not mutually exclusive:

| Idea | Means | Settled by |
|---|---|---|
| **Job identity** | An independently meaningful accomplishment: a functional job | At the boundary, by the topology (and job domain analysis where open); inside a job, by the job map |
| **Decomposition** | A smaller undertaking that contributes to a larger one; a **sub-job** has identity *and* is part of a larger job | Proposed as constituent candidates by the topology; classified by the job map |
| **Episode** | An occurrence of a job, with its trigger | Noticed by the topology (as constituent candidates); classified by the job map |
| **Relationship** | A dependency or interaction between distinct jobs | Described in words in the topology; classified in job domain analysis |

A shared higher-level objective is evidence that jobs are related, not that they are one; a trigger and a completion
do not make a job (steps have both); and a different success criterion is an outcome, not a job.

## Generic activity model

Most activity-modelling techniques share one structure: **units of activity, decomposed into smaller ones, performed
by someone, acting on things the domain names, related to one another, judged by criteria, and varied by case**. They
differ mainly in what they call the units, which classifications they impose, which links they allow, what extra facts
they record and what constraints they add.

The model holds only that shared structure, and says nothing about any one technique. Everything particular to a
technique is supplied by a **profile** (below).

Activities and performers belong to a **domain**, not to the document that first names them. A document (an
`ActivityModel`) is a view onto its domain: it refers to the activities it is about, and may propose new ones. So an
activity exists as soon as any document names it, several documents can refer to the same activity, and one document
can be agreed as the authoritative list of the domain's activities without being their only container. The domain is
the same one the glossary uses (the folder that stands for the domain), so activities, performers and terms share one
scope. Jobs to be Done, as this family practises it, is one configuration of
three profiles ([The model configured for Jobs to be Done](#the-model-configured-for-jobs-to-be-done)); other
techniques are further profiles, added without changing the model.

*Activity* is the generic unit. It is not the glossary's Activity kind, which is a word the domain uses; an activity
here may involve several such words.

```mermaid
classDiagram
    direction LR

    class Domain {
        name
        description [0..1]
    }
    class ActivityModel {
        title
        profile
        description [0..1]
        properties [*]
    }
    class Activity {
        name
        statement
        description [0..1]
        status
        category [0..1]
        variantKind [0..1]
        appliesTo [*]
        position [0..1]
        intent [0..1]
        source [0..1]
        notes [0..1]
        properties [*]
    }
    class Performer {
        name
        capacity
        rationale [0..1]
    }
    class ActivityLink {
        kind [0..1]
        description [0..1]
    }
    class Criterion {
        statement
        kind [0..1]
        notes [0..1]
        properties [*]
    }
    class Qualifier {
        kind
        text
    }
    class Seam {
        kind
        text
    }
    class Term {
        <<glossary>>
        preferredWord
    }
    class SyncBinding {
        id
        version
        lastUpdated
    }

    Domain "1" *-- "*" Activity : activities
    Domain "1" *-- "*" Performer : performers
    Domain "1" *-- "*" ActivityModel : models
    Domain "*" --> "*" Term : glossary
    ActivityModel "*" --> "*" Activity : covers
    ActivityModel "*" --> "0..1" Activity : focus
    Activity "*" --> "0..1" Activity : partOf
    Activity "*" --> "1" Performer : performedBy
    Activity "*" --> "*" Term : actsOn
    Performer "*" --> "0..1" Term : agent
    Activity "1" *-- "*" ActivityLink : links
    ActivityLink "*" --> "1" Activity : to
    Activity "1" *-- "*" Criterion : criteria
    Activity "1" *-- "*" Qualifier : qualifiers
    Activity "1" *-- "*" Seam : seams
    Activity "1" *-- "0..1" SyncBinding : sync
```

### Elements

| Element | Notes |
|---|---|
| **Domain** | The scope everything else belongs to: the area of the business being analysed, the same as the glossary's domain (in documents, the folder that stands for it). It owns the activities and performers, and holds the documents about them. An activity is identified by its `name` within its domain. |
| **ActivityModel** | One document of one profile (a job map, a value chain, a story map), in a domain. `profile` names the profile, and so the labels, values, properties and constraints that apply. `covers` are the domain's activities the document is about or names; `focus` is the one it is centred on. `description` is its opening prose. A document can name an activity the domain did not yet have; it is then added to the domain as proposed. |
| **Activity** | The generic unit, owned by its domain. `name` identifies it within its domain; `statement` is its full form; `description` says what it covers, without breaking it into sub-activities. `category` is a value from the profile's classification. `position` orders it among its siblings where the profile gives order a meaning. `intent` is the result its performer is pursuing: what distinguishes one activity from another. `status` is `proposed` (named by a document, not yet agreed) or `agreed` (accepted into the document the profile treats as authoritative); a profile says which document that is. |
| **partOf** | Decomposition: an activity that is part of a larger one, in the same model or another. Whether the part keeps an identity of its own is for the profile to record. Profiles limit the depth. |
| **Variants** | A **variant** is an activity that says what another activity (its **core**) must accomplish, or what changes, in a particular case: it is `partOf` its core, shares its `category`, and has a `variantKind` and an `appliesTo` naming the case. Kinds are profile-defined (a situation, a particular kind of thing, a market, a channel). `appliesTo` names one case or several sharing the same statement, as text kept consistent by the profile's naming rule, not a separate entity. A variant never changes its core's intent. |
| **Performer** | Who performs an activity, by `capacity` (the responsibility carried), not title; resolves to an agent term in the glossary. `rationale` records what was unified or split, and why. |
| **actsOn** | The glossary nouns an activity's statement uses. In documents these are words in the statement, not a field; drift checks compare them with the glossary. |
| **ActivityLink** | A link between two distinct activities, other than decomposition. `kind` is a profile-defined value (a relationship, a sequence, a dependency), and may be absent where a profile describes links in words; `description` says what the link is. |
| **Criterion** | How success of an activity is judged. `statement` is the criterion as written; `kind` and `properties` carry any form the profile imposes (an outcome statement's parts, an acceptance criterion's conditions, a service level's target). `notes` holds what must survive agreement about the criterion itself (to be validated; derived from a qualifier; its measure to be settled). |
| **Qualifier** | A further dimension of an activity that holds whatever the case (an emotional or social aim, a regulatory note); `kind` is profile-defined. A profile may require qualifiers to be turned into criteria. |
| **Seam** | Where execution leaves any system: it `happensInWorld`, `arrivesFromWorld`, or runs `bothWays` (the act inside gives the change outside its effect). |
| **properties** | Profile-defined facts recorded on a model, an activity or a criterion, as a name and a value. A value may be simple (a word, a number), a structured record with named fields, or a list of either. The model fixes only that they exist; each profile declares which properties it uses, where, their fields, and what they mean. |
| **SyncBinding** | Present only when synced with an external system; never invented. In documents it is the YAML block under an entry's heading. |
| **Evidence** | Not in the model: evidence marks (attested, inferred, proposed as a modelling choice) belong to drafts and are dropped on agreement. They are not an activity's `status`, which records only whether it has been agreed. Open questions are text in `notes`, prefixed `Open:`. |

### Profiles

A profile configures the model for one technique. It declares:

- what it calls the model and the activity, what the model's `focus` is, and which of its documents is authoritative
  for an activity's `status`;
- its `category` values, and how deep `partOf` may go;
- its link kinds, and between what they run;
- which variant kinds and qualifier kinds it uses, and its naming rule for `appliesTo`;
- the form of its criteria;
- the properties it records, and where;
- the constraints that tie them together.

Adding a technique is a matter of writing those down, not of changing the model. For example (illustrations of the
pattern, not skills in this plugin):

| Technique | Activity is | category | partOf | ActivityLink | Criterion |
|---|---|---|---|---|---|
| Value chain (Porter) | Activity | Primary, support | Optional: activity → sub-activity | Not used | Not used |
| Hierarchical task analysis | Goal, subgoal, operation | Level | Recursive, any depth | Plan (when each sub-task is done) | Performance standard |
| User story map (Patton) | Activity, task, story | Backbone, walking skeleton, release | Activity → task → story | Sequence along the backbone | Acceptance criteria |
| Process model (swimlane, BPMN) | Process, step | Task, decision, event | Process → step | Sequence, condition, message | Service level |
| Event partitioning (essential systems analysis) | Planned response | External, temporal event | Response → step | Triggered by (an event) | Not used |

## The model configured for Jobs to be Done

The job family configures the generic model as three profiles: the **job topology**, **job domain analysis** and the
**job map**. They share one set of values and properties, declared once here.

**Jobs belong to the domain; the topology is the agreed view of them.** A job named by any document (a map's focus
job made before any topology exists, a higher-order job, a stakeholder job a map finds) is a job of the domain, with
`status: proposed`. It becomes `agreed` when it is accepted into the topology, which remains the authoritative list of
the domain's jobs and executors. A step is an activity of the domain too, but belongs to its map: its `status` follows
its map's agreement. The skills remain the authority on what
each value means in practice; this section says how they land in the model.

### The three profiles

| Model element | Job topology | Job domain analysis | Job map |
|---|---|---|---|
| ActivityModel | Topology (one per domain); authoritative for jobs' `status` | Analysis (one per domain, optional; refers to the domain's jobs) | Job map (one per job mapped) |
| focus | The main job | The main job, or the jobs taken up | The job mapped: any job of the domain; one not yet in a topology is `proposed` |
| Activity | Job (and sub-jobs) | Job | Step, and its variants; may also propose jobs (higher-order, stakeholder, separately mappable) to the domain |
| Performer | Job executor | The topology's executors | The focus job's executor |
| intent | The job's desired result; with `successCriteria` and `scope` kept beside the statement | As the topology | Not used: a step serves its job's intent |
| partOf | Sub-jobs to the main job; constituent candidates are noted on the main job's entry | Not used | Every step to the focus job; variants to their core step |
| position | Not used | Not used | Order within a stage, as the executor would describe it; the stage gives the grouping |
| ActivityLink | Related and stakeholder jobs to the main job, in words; `MeansTo` from the main job to a higher-order job | Classified relationships, each to the most specific job it bears on | `MeansTo` from the focus job to a higher-order job it proposes |
| Criterion | Not used | Not used | Desired outcomes, usually two to four per significant step once researched |
| Qualifier | Emotional and social, on jobs | Not used | Turned into criteria on the steps they bear on |
| Variants | Circumstances on jobs | Not used | `EdgeCase` and `Circumstance` variants of core steps, only where the step changes |
| Seam | Flagged (`flags`) | Direction settled | Marked on steps |

### The eight stages

The job map's `category` is one of Ulwick's eight universal stages. A step is placed by its functional purpose, not by
when it happens; the stages organise an inventory, not a sequence.

| Stage | The executor must… |
|---|---|
| `Define` | determine what needs to be done, considered or achieved |
| `Locate` | gather the inputs, information, resources or items required |
| `Prepare` | arrange or ready what is needed |
| `Confirm` | verify readiness, assumptions, conditions or prerequisites |
| `Execute` | perform the central activity: the actions that accomplish the job |
| `Monitor` | assess progress, state, performance or emerging conditions |
| `Modify` | adjust in response to a problem that has been found |
| `Conclude` | complete the job, or a piece of work within it, and establish the resulting state |

### Values and kinds

| Declared | Values |
|---|---|
| `category` (topology) | `Main`, `SubJob` (a constituent the job map found separately mappable), `Related` (the same executor's other job, in Ulwick's sense), `Stakeholder` (another executor's job that touches the main job) |
| `category` (domain analysis) | The topology's categories, for the jobs it refers to |
| `category` (job map) | The eight stages, above |
| `variantKind` | `Core` (default), `EdgeCase` (a particular kind of thing the job deals with; `appliesTo` is the glossary's preferred word), `Circumstance` (a situation the whole job is done in; `appliesTo` is its label as listed with the map) |
| `ActivityLink.kind` | Domain analysis: `Changes`, `Enables`, `Constrains`, `Governs`, `Consumes`, `RespondsTo`. Topology: otherwise described in words; a related job may be `Before`, `After` or `Alongside`. Topology and job map: `MeansTo` (the focal job is one means to a higher-order job: buying a property to *secure a place to live*) |
| `status` | `proposed`, `agreed`; a job is agreed when accepted into the topology |
| `Qualifier.kind` | `Emotional`, `Social` |
| `Criterion` | Job map only: a desired outcome, with properties `direction` (minimise, increase), `measure` (time, likelihood, variability, number, effort), `object`, `clarifier`; `notes` for what must survive agreement (to validate, as for an outcome that encodes a decision strategy; derived from a qualifier; measure to settle) |

### Properties

| Property | On | Profile | Meaning |
|---|---|---|---|
| `constituents` | The main job | Topology | Each constituent candidate, with its `trigger`, what was noticed, its `lean` (likely an episode, likely a step, possibly a job, unclear) and its `status` (open, or the map's classifications) |
| `scope` | A job, chiefly the main job | Topology | What the job's object takes in and leaves out, kept out of its statement |
| `successCriteria` | A job, chiefly the main job | Topology | How the executor judges the whole job, kept out of its statement; not desired outcomes |
| `edgeCases` | The main job | Topology | The cases its object's breadth was tested against, each with its finding |
| `identity` | A job taken up on a boundary question | Topology, domain analysis | One job or two; part of the main job or beside it; one executor or two; with the five tests' findings behind it |
| `standard` | Any activity whose result is assurance | All | `consistency` or `correctness` |
| `openClassifications` | The model | Topology | Boundary questions the five tests genuinely split on, each with its evidence |
| `subDomainHypotheses` | The model | Topology | Each, with the signal that prompted it |
| `boundaryQuestions` | The model | Topology | Questions about the main job's edge left open |
| `flags` | The model | Topology | Seams, obligations and supplying, for deeper analysis |
| `mapping` | The model | Job map | Over its life (the default), or a sub-job on its own |
| `circumstances` | The model | Job map | The circumstances the job is done in, declared once: each with its `label` (C1, C2, …) and `description`; a `Circumstance` variant's `appliesTo` names one |
| `episodes` | The model | Job map | For a continuing job, each episode with its trigger and the steps it uses; a step entry's *Episodes* is the inverse view |
| `classifications` | The model | Job map | Each constituent candidate: `covered` (with the steps), `separatelyMappable`, `outsideScope`, `unresolved` (with why); covered and separately mappable may both hold |
| `coverage` | The model | Job map | Each circumstance, and each significant edge case: the steps that cover it, and the finding (covered, a gap, an ambiguous boundary, possibly another job) |
| `order` | A step | Job map | Where it helps: that the step runs alongside another, repeats, is done on demand, or returns to another step. Never a required sequence |

### Constraints

**Job topology**

- Exactly one main job.
- The topology is the agreed view of the domain's jobs: a job is `agreed` once it is in the topology, and `proposed`
  until then, whichever document named it.
- A related job has the main job's performer and a different intent; a stakeholder job has a different performer.
- Performers are one only if they pursue the same intent, never because they stand to another activity the same way;
  two stakeholder jobs with the same relationship to the main job but different intents remain separate.
- A different motivation for the same functional objective is not a different job; a higher-order job the focal job is
  one means to is a different job, not a restatement of it.
- Work that seems to make up the main job is recorded as constituent candidates, with a lean but no verdict, until a
  job map classifies it.
- Boundary questions the evidence does not settle go in `openClassifications`, not forced; a shared higher-level
  objective never settles identity on its own.
- The topology is the authoritative list of jobs and executors, updated when a map's classifications and proposed
  jobs are agreed. A higher-order job is recorded with a `MeansTo` link from the main job, not used to restate it.

**Job domain analysis**

- It refers to the topology's jobs and does not define its own.
- It works between jobs and leaves their internal structure to their maps.
- Identity is settled by weighing the five tests, never by a shared objective, performer, trigger, source or success
  criterion alone.
- Every relationship has a kind and runs to the most specific job it bears on.
- Changes to the topology are proposed there, not made here.

**Job map**

- One focus job, a job of the domain: agreed in the topology, or `proposed` where the map is made before one exists.
  Every step has the focus job's performer (delegated work stays the performer's).
- Circumstances are declared once, in `circumstances`; every `Circumstance` variant names one of them.
- Jobs the map finds that are not its own (higher-order, stakeholder, separately mappable) are proposed to the domain,
  for the topology to agree; the map does not make them agreed.
- One level of steps; a core step may have variants (part of it, in its stage, with a `variantKind` and an
  `appliesTo`, and no variants of their own).
- Each step is placed in a stage by its functional purpose, none filled for its own sake; Execute is not defined by
  irreversibility, and Confirm need not precede it in every circumstance. Steps are presented grouped by stage.
- The steps are an inventory, not a sequence, and need not all be used by any one occasion of the job. A step that a
  different method would remove without losing a necessary accomplishment is a means, not a step.
- A job is mapped over its life by default, with circumstances and edge cases as variants of the steps they change.
  Completeness is tested by coverage of each circumstance.
- Every constituent candidate is classified, and each classification is reported to the topology without holding the
  map up. Separate mappability is judged by objective, never by a sequence of its own; overlap with the parent's map
  is expected. Granularity is judged by the focal job's objective, never by counting steps.
- Criteria take the outcome form; their completeness is judged separately from the steps', they are checked against
  the executor's capacity and the domain's causal rules, and tensions between them are recorded, not resolved.
- Conclude steps must be accomplishments the job needs. The choice of map never changes what the jobs are.

## Mapping to other systems

- **Matching.** Use an external system's identifier once it has one (`SyncBinding.id`); until then match on an
  activity's `name` within its domain.
- **Scope.** Map the domain to the target's container for a body of work (a project, a space, a folder); activities
  and performers are created there, and each document refers to them rather than copying them.
- **Status.** Carry `proposed` and `agreed` as a status or tag, so a proposed job is not read back as agreed.
- **Hierarchy.** Most tools hold a tree (initiative → epic → story, process → step, job → step). Map `partOf` to it and
  `category` to a type or tag, and keep the profile so the tree can be read back with the right labels.
- **Variants.** Map a variant to a child record, note or conditional field of its core activity, keeping its
  `variantKind` and `appliesTo` (as a tag or condition). Where the target has none of these, write variants into the
  core activity's description as `<appliesTo>: <statement>`, so they can be read back.
- **Properties.** Map profile properties to custom fields where the target has them; otherwise to tags or a structured
  block in the description, keeping their names so they can be read back.
- **Links.** Keep the link kind; where the target has only untyped links, carry the kind in a custom attribute.
- **Criteria.** Tools built around Outcome-Driven Innovation hold jobs, steps and outcomes natively; elsewhere criteria
  map to child records or a structured field of their activity, never pooled at a higher level.
- **Versions.** Before pushing, compare `version` or `lastUpdated` with the external record and stop on a mismatch.
