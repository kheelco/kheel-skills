# Steps

## What a job map is

A job map is a **structured inventory of the functional accomplishments required to get a job done, organised by
Ulwick's eight stages**. It is not an execution workflow. Its **completeness** is judged by whether it covers the job
across the circumstances it is done in ([Coverage across circumstances](#coverage-across-circumstances)); its
**coherence** by whether each step makes a functional contribution to the job and sits in the stage that contribution
belongs to ([Placing a step in a stage](#placing-a-step-in-a-stage)). Neither depends on the steps forming a single
sequence.

- **Stages organise by function, not by order of execution.** The stages run roughly from defining the job to
  concluding it, and an executor will usually describe the steps in that order, but the map does not require them to
  form a continuous path, every occasion of the job to pass through every stage, or Monitor to follow Execute. A
  continuing job's steps may be carried out continuously, periodically or on demand, and any one occasion uses only
  the steps it needs.
- **Its own sequence does not make a job.** Work with its own order of steps, its own trigger or its own completion
  (checking the record, correcting it) may still be steps of this job. Whether something is a job of its own is judged
  by its objective ([Constituents, and jobs found while mapping](#constituents-and-jobs-found-while-mapping)), never
  by its having a sequence.
- **No quotas.** No step per stage, no equal numbers across stages, no single Execute step, and no requirement that
  every stage yields a step.

An **operating cycle** (receive → validate → update → verify → correct, read as the handling of one event) is a
workflow, not a job map: it records the order of operations for one case rather than the accomplishments the job
needs across all of them, and usually presupposes a mechanism.

## The eight stages

Outcome-Driven Innovation names eight universal stages. They are a **completeness framework for discovery**, a set of
questions to ask about any job, not eight boxes to fill.

| Stage | The executor must… | Ask |
|---|---|---|
| **Define** | determine what needs to be done, considered or achieved | What do they have to work out before anything can start? |
| **Locate** | gather the inputs, information, resources or items required | What do they have to have to hand, and where does it come from? |
| **Prepare** | arrange or ready what is needed | What has to be set up, structured or made ready? |
| **Confirm** | verify readiness, assumptions, conditions or prerequisites | What do they check before committing? Who has to have agreed? |
| **Execute** | perform the central activity of the job | What is the act that, once done, cannot be undone cheaply? |
| **Monitor** | assess progress, state, performance or emerging conditions | What do they watch, and how do they find out whether things are as they should be? |
| **Modify** | adjust in response to a problem that has been found | What goes wrong, and how do they put it right? |
| **Conclude** | complete the job, or a piece of work within it, and establish the resulting state | How do they know it is finished, and what is left behind? |

A stage may yield no step, one, or several. **Present the steps grouped by stage**, in the eight stages' order,
whatever order they were found in; within a stage, in the order an executor would describe them. The grouping is for
reading, not a claim about the order of execution. Where it helps to understand a step (it runs alongside another,
repeats, or is done on demand), say so in its notes.

## Placing a step in a stage

Assign a step to a stage by its **functional purpose**: the contribution it makes to getting the job done, and why
that contribution belongs to that stage. Not by when it happens, what it is called, or a resemblance to the stage's
name. Most placements are obvious and need no justification; take care with these:

- **Monitor** assesses the state, progress or conditions of what the job produces or maintains (*establish whether
  the register agrees with its sources*). It need not follow Execute.
- **Modify** adjusts in response to a problem that Monitor, or the work itself, has shown: obtaining corrected inputs,
  resolving conflicting instructions, adjusting what is about to be done, stopping, or, in a continuing job, putting
  the maintained state right where it is in error. Where it helps, say what it returns to; it need not be the next
  link in a chain. In a map of a sub-job it adjusts that sub-job's work; an error that predates it belongs to the
  parent job's Modify, or to whichever job corrects it.
- **Conclude** brings the job, or a piece of work within it, to completion and establishes the resulting state
  (*establish that the register states the current position*). It does not mean *what happens when the object comes
  to an end*. Finalising or preserving the object at the end of its life is a Conclude step only where that is part
  of this job; it may instead be another job (winding up, archiving), which goes to the topology. Test every Conclude
  step: **is it a functional accomplishment the job needs** (the resulting state established, work handed over, a
  record left that the job depends on), **or an ending added because maps are expected to have one?** A continuing job
  may have Conclude steps for pieces of its work, or none; an empty Conclude stage is better than a forced one.
- **Confirm before Execute.** Confirm establishes readiness and authority; Execute is the commitment that cannot be
  undone cheaply. Keep checks out of Execute and commitments out of Confirm.

**Where placement is ambiguous, say so.** Holding back a change whose conditions are not met may be Confirm
(establishing the conditions before committing) or Modify (responding to a failed confirmation), depending on how the
step is stated. Record the competing readings and the one chosen in the step's notes, rather than forcing it
silently.

## Finding the steps

- **Only necessary accomplishments.** Introduce a step only when it is something the executor must accomplish to
  achieve the job's desired result, in some circumstance the job is done in. Never create a step to populate a stage;
  an empty stage is better than an artificial step.
- **Every step serves the job.** Test each step against the job's desired result (and, in a map of a sub-job, its
  completion). Where work is handed to another executor (a dispute referred to a tribunal), the steps stop at the
  hand-off: identify, document and refer, not settle.
- **Density.** A job map typically has ten to twenty steps, several under some stages and none under others. Fewer
  usually means steps stated too broadly; many more, a job stated too high. This is guidance, not a rule.
- **An empty stage is a prompt.** A stage that yields nothing is allowed. Ask whether the work it would hold was put
  under a neighbouring stage, or whether the job's boundary is drawn so that the work falls outside it, and record
  what the empty stage suggests.

## Pre-check: which job, and how to map it

A job map maps **one functional job**, chosen from the job topology (the `job-topology` skill), with its executor and
its desired result. Confirm the job is in the topology and its executor settled; if not, settle them there first. Take
in the topology's **constituent candidates** for the job (work that seems to make up the main job, each with what was
noticed and a provisional lean; they are recorded on the main job only, so a related job mapped on its own has none),
the circumstances and edge cases recorded on the job, and any open boundary questions the map depends on.

By default the job is mapped **over its life**: one map holding the steps the executor must accomplish to get the job
done across every circumstance it is done in, not one transaction. **Circumstances** and **edge cases** are folded
into the steps they change ([Circumstances and edge cases](#circumstances-and-edge-cases)).

## Constituents, and jobs found while mapping

As the map takes shape, consider each of the topology's constituent candidates, and any other undertaking that looks
as if it might deserve a map of its own, and classify it:

| Classification | Meaning |
|---|---|
| **Covered** | Its functional work is represented within this map; say by which steps |
| **Separately mappable** | It appears to have a distinct functional objective worth mapping on its own |
| **Outside scope** | Its objective belongs to another job (a related or stakeholder job, or one beside the main job) |
| **Unresolved** | Its relationship to the job is still uncertain, or it has not been examined yet; say which |

**Covered and separately mappable can both hold.** A map works at one level. Taking in a change can be represented by
several steps of this map and still be worth a map of its own at a finer level, whose steps are what must be
accomplished to take a change in and whose outcomes measure that. The two maps are at different levels: this map keeps
its steps and outcomes, and the finer map breaks the same work down further.

**Overlap is expected, not a reason to reject.** A finer map of covered work will overlap with this one, since it
covers the same ground in more detail. That overlap is never, on its own, grounds for rejecting separate mappability:
judge the candidate by its objective. Only where a separate map would add nothing (the same steps at the same level,
with the same outcomes) is the candidate covered and nothing more.

**Separately mappable is judged by objective, not sequence.** The candidate has a functional objective the executor
sets out to achieve and would judge on its own, and a map of it would find steps and outcomes this map does not hold.
Weigh the topology's five tests (independent objective, independent completion, executor, context independence,
stable identity), the objective most of all. Its own sequence, trigger or completion does not establish it, nor does
being separately completable, and **a different success criterion is not a different job**: consistency and
correctness, or speed and accuracy, are outcomes on the same steps unless each is pursued as an accomplishment of its
own.

**Do not hold the map up for them.** Classifications are findings, not gates: the map proceeds with candidates
unresolved or separately mappable, and a separately mappable candidate is mapped only when that is worth doing.
Report every classification to the topology (*covered: Monitor*; *covered: Locate to Execute, and separately
mappable*; *unresolved: not examined*), where the candidate's status is updated. A classification is a reason to
revise the topology, not proof that it was wrong. An undertaking found while mapping that the topology never listed
goes back as a new candidate.

**The granularity check.** If several candidates are separately mappable and together account for most of the map,
ask whether the focal job is the right unit for a job map at all, or a **higher-order objective** containing several
mappable jobs. If it is, say so: the topology may restate it.

Never split a job into several maps by episode, trigger, source, sequence or success criterion alone, and never let
the convenience of a map decide what the jobs are.

## Step rules

Each step says **what the executor is trying to accomplish** at that point, not the operation they perform, and not
how the current process or software makes them do it. Ask of each step: *what do they have, once this is done, that
they did not have before?* A step that can only be answered with *the operation is done* is an operation, not a
milestone.

| Prefer | Over |
|---|---|
| Determine which obligations apply to the organisation | Search the obligations register and select applicable obligations |
| Confirm that the change is permitted | Run the restriction check |
| Establish the vehicle is safe to return to use | Close the work order in the system |

- **A milestone, not a task.** Something that is either accomplished or not.
- **Timeless.** Name a particular system, product, document or instrument only as an example of a circumstance or an
  output, marked as such, never in the step statement itself.
- **Verb + object**, in the executor's own language, the object a glossary noun, with a clarifier only where two steps
  would otherwise read alike.
- **The job's executor.** Every step is accomplished by the executor of the job. A step that someone else accomplishes
  is part of their job: a stakeholder job in the topology. The executor may depend on others (a committee's approval arrives);
  the step is then what the executor must accomplish about it (*confirm the change has been approved*).
- **One question per step.** A step whose outcomes answer different questions (whether the action is authorised;
  whether the people and things affected are eligible for it) may be two steps. Split it where that makes the map
  clearer, or keep one step with its outcomes plainly grouped; either way, do not let one question stand in for the
  other.
- **What it covers, not sub-steps.** Where a step spans several things the executor must establish (the classes, the
  number of each, their rights and restrictions), say so in the step's **Covers**, not as sub-steps; if the things are
  separate accomplishments, make them separate steps under the same type.
- **One level.** A job map breaks a job into steps, not steps into sub-steps. A step's circumstances and edge cases
  (below) are variations of it, not sub-steps. A step that needs its own breakdown is a
  sign the job was stated too high, or that the step is really a job.

## Circumstances and edge cases

Both are **cases** in which a step must accomplish something more, or something different, than it does ordinarily.
They are kept apart because they are found and used differently:

| | Circumstance | Edge case |
|---|---|---|
| What it is | A situation the **whole job** is done in | A particular **kind of thing** the job deals with |
| Examples | A first set-up; a large organisation at volume; a contested case; a recovery | A joint holding; a partly paid share; a deceased member; a family membership |
| Where it is declared | Once, with the map (C1, C2, …), from the circumstances on the job in the topology | On the step it changes, usually naming a glossary term |
| What it touches | Often several steps | Usually one or two steps |

On each step it changes, a case is written as **`<case>: <what the step must accomplish in that case>`**, still
solution-free and from the executor's side:

- *Joint holding: confirm that every joint holder has authorised the disposal, or the survivors' right where one has
  died.*
- *C3 (contested): confirm what the tribunal has decided before going further.*

Rules:

- **Name the case in the domain's words, and the same way every time.** An edge case is named by the glossary's
  preferred word (*Joint holding*, *Partly paid share*); one the glossary does not hold is a candidate term. A
  circumstance is named by its label exactly as listed with the map (*C3 Corporate action*, or *C3*). The edge cases tried in the topology, when testing the
  breadth of the job's object, are the first place to look for them.
- **Only where the step changes.** A case belongs on a step only if the executor must accomplish something more or
  different there; one that changes nothing is not recorded.
- **A case can yield outcomes.** Where the case is where things go wrong, write its outcomes on the step in the usual
  form (*minimise the likelihood that a disposal is entered without every joint holder's authority*).
- **A case is not a step or a map.** If what the case requires has its own place in the job (it must be accomplished
  for every instance, not only this kind), it is a step; if it pursues a different result, it is another job.
- **Circumstance or edge case?** If it describes the situation of the whole job (who, how much, in what state of
  dispute), it is a circumstance; if it describes the thing being dealt with, it is an edge case.

## Coverage across circumstances

A map's completeness is tested against the job's circumstances and edge cases, not by tracing paths through it. For
each circumstance listed with the map, and each significant edge case, ask: **does the map contain the functional work
needed to get the job done in this case?** The question is not *which steps happen, in what order*. For example:

| Circumstance | Coverage question |
|---|---|
| A first set-up | Does the map account for establishing the initial state? |
| A change of executor | Does it account for taking over responsibility for an existing state? |
| An action affecting many things at once | Does it cover a change to many items together, not only one at a time? |
| A contested case | Does it cover uncertainty, and the limits of the executor's authority? |
| Volume, or automated arrival | Do the steps still hold when the work arrives in bulk or through automated means? |
| The end of the object's life | Is there a genuine functional step (finalising, preserving), or is that another job? |

Record what each test finds, briefly: covered (by which steps, or which cases on them), a **missing step** (add it, or
record the gap), an **ambiguous boundary**, or a sign that the circumstance is **another job** (back to the topology).
Do not construct a workflow for each circumstance.

## Execution seams

Where a step's execution happens outside any system (the negotiation, the payment, the signature, the court order), say
so on the step: whether it **happens in the world** (the executor does it, but not through any system) or **arrives
from the world** (the executor receives its result). The map is then honest about what software could support or
perform, and what it can only receive.

Where the topology says a seam runs **both ways** (recording gives the change its effect), keep two questions apart in
the steps: *what should the record say, given the position?* and *what position results from making the entry?* A
Confirm step then confirms the entitlement to make the change (not that the change has already happened), and the
Execute step has consequences outside the record. Test the steps against a case where the entry is what makes the
change, not only against one where it records a change already made, and treat that effect as a claim to be checked
against its source.

## Assurance: jobs and steps that check

A job or a step whose result is assurance (verifying, checking, validating, auditing, reconciling; often a continuing
job's Monitor) must work to a named **standard**, the one the job's statement implies ([topology](../../job-topology/references/jobs.md), *The core functional job*):

- **consistency**: the steps establish whether the thing agrees with the evidence available for it, and the
  completion is a statement of agreement and disagreement;
- **correctness**: the steps must also establish whether the available evidence is **sufficient** to show the
  underlying state is right: what is missing, what conflicts, what was derived from the thing being checked, and what
  happened but was never evidenced. The completion is justified confidence, or a stated limit to it.

A map that compares a thing with its sources and then claims correctness has done consistency work. Where the
standard is not evident, settle it with the topology before mapping; where both are needed, they are
separate outcomes, or separate steps where each needs work of its own, not separate jobs.

## A step is not a glossary activity

A step is an analytical construct: a milestone in getting this job done. A glossary activity (*Audit*, *Settlement*,
*Admission*) is an act the domain itself names and talks about. One step may involve several such activities; one
activity may recur across several steps and several jobs. Do not copy the map into the glossary as activities, or the
glossary's activities into the map as steps. A step's nouns should be glossary terms; its verb is the executor's.

## Errors to watch for

- **Flow required.** Steps judged by whether they form one sequence: a step questioned because it does not follow the
  one before, or every occasion of the job required to pass through every stage.
- **A job from a sequence.** Work made a separate job, or a separate map, because it has its own order of steps,
  trigger, source, completion or success criterion.
- **Candidates forced.** A candidate made either covered or separately mappable when both hold; a classification the
  evidence does not support; the map held up until every candidate is settled; classifications not reported to the
  topology.
- **Rejected for overlap.** Separate mappability refused because a finer map would overlap with this one, without
  asking whether the candidate has a distinct objective. (Only a map that would add nothing at all is redundant.)
- **Placed by timing or name.** A step put under a stage because of when it happens, what it is called or how it
  resembles the stage; Conclude used for *what happens when the object ends*, or added as a universal ending the job does not need; an
  ambiguous placement forced silently.
- **Stages as buckets.** Steps placed under a stage because it needed filling, or a step per stage, several of them
  thin. The stages are questions, not slots.
- **Coverage untested.** Circumstances listed with the map but never tested against it; or a workflow drawn for each
  circumstance instead.
- **Work past the hand-off.** Steps that do the receiving job's work.
- **An empty stage passed over.** No step under a stage, with no look at whether the boundary put its work elsewhere.
- **A process map in disguise.** Steps that name today's documents, systems and hand-offs. Ask what each is for.
- **A stakeholder job's steps in the map.** The auditor's verification appearing as a Monitor step. Different
  executor; back to the topology.
- **Steps that are glossary activities transcribed.** *Admit* as a step because the glossary has *Admission*.
- **Assurance without a standard.** A map that compares with sources and claims correctness, or names no standard.
- **Sub-steps.** A step broken into steps of its own: the job is too high, or the step is a job.
- **Forty steps.** The job was stated too high, or the map has taken in its related jobs.
- **Seams left unmarked.** A map that reads as though a system did everything.
- **Cases mislaid.** A circumstance recorded as an edge case or the reverse; a case recorded on a step it does not
  change; an edge case named in words the glossary does not hold, and not sent to it.
