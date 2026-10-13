# Executors and jobs

## The executor

Define the executor by their **capacity**: the responsibility they carry in getting the job done (*the person or
organisation responsible for maintaining the company's record of share ownership*), not a title, office, department,
seniority or persona. Give the executor a convenient **name** (*Company secretary*), an agent term in the glossary, but
do not let the name assume a formal office the domain does not always have: many companies have no appointed secretary,
and the job is still done. Where no existing word fits and a name is coined for the capacity, its glossary entry says
it names a functional role, not a formal or statutory office, so readers do not take it for one.

- **Unify when the desired outcome is the same.** People getting the same job done, trying to achieve the same result,
  are one executor, however different their scale, volume, infrastructure, frequency, seniority or obligations. An
  in-house secretary, a director doing it themselves and an outsourced provider are one executor; so, at first, is a
  registry operator for a listed company, whose differences (volume, settlement interfaces, corporate actions,
  regulation) are **circumstances** of the same job.
- **Split only when the desired outcome changes.** Where the intent or the shape of the job is materially different, it
  is a different executor, and usually a different job. A CFO modelling a capital structure is not the company
  secretary at a higher level: the intent (*what if* against *what is*) and the lifecycle (throwaway against permanent)
  differ. More steps, more volume or different infrastructure are not reasons to split.

Record, for each executor, a line on what was unified or split and why.

## Roles are not jobs

An executor's role often spans several jobs, and coordinating someone else's job does not make it theirs. The company
secretary may organise a share issue, draft its resolutions and chase its payments; that does not put the share issue
in the secretary's job. Ask, of each thing the executor does: **is this getting their job done, or helping someone else
get theirs done?** Help given to another job is, at most, a step of the executor's own job (*confirm the issue has been
authorised*) or a sign of a related job.

## The core functional job

State it as **verb + object + contextual clarifier**: *Maintain* an accurate, legally compliant *record of who owns the
company's shares* *over the life of the company*. The verb and object, without the clarifier, are the job's **name**,
which identifies it (*Maintain the record of share ownership*).

It must be free of any solution, independent of current technology, stable enough to outlive any process, stated from
the executor's perspective, and about something they are trying to accomplish.

### Altitude and breadth

- **Would it still be the job under a completely different process?** If not, it is too low.
- **Does it have a beginning and an end, or a standing state with recurring work?** If neither (*run the company*), it
  is too high. If a standing state, see *Continuing jobs* below.
- **Is there one executor for it?** Two executors in one statement is usually two jobs.
- **Is the object the right breadth?** Test it against edge cases from the domain, cases at the edge of what the
  executor must keep coherent (for share ownership: a subdivision, a conversion between classes, partly paid shares, a
  cancellation). If the executor cannot handle them without artificial distinctions, the object is too narrow (*share
  ownership* where *share capital and its ownership* is meant). If widening it brings in several independent results,
  it is too broad. Record the cases tried and what they showed.

### Continuing jobs and their episodes

Some jobs have a beginning, execution and end (*settle an estate*). Others are **continuing**: they keep something in a
desired state indefinitely (*maintain the record of share ownership*). A continuing job is legitimate, and often the
right main job, because its intent is the standing state, not any one piece of work. It shows in the work the executor
does when nothing new arrives: an error found after two years of quiet, a discrepancy with old documents, a disputed
holding, a reconstruction after loss, a question about ownership on a past date.

A continuing job is done through **episodes**: recurring or exceptional executions of part of the job, each with a
trigger.

| Trigger | Example episode |
|---|---|
| **Event-driven**: something arrives | Incorporate a change in share ownership |
| **Periodic**: a cycle comes round | Verify the accuracy of recorded ownership |
| **Exceptional**: something is found wrong | Correct an ownership record |

Episodes are **not separate jobs**. They have the main job's executor and intent, and they are recorded on the main
job's entry, each with its trigger.

**Keep episodes at one altitude.** Episodes are the recurring or occasional modes of keeping the state, each a modest
piece of work. An exceptional undertaking big enough to have its own beginning, execution and end (rebuilding the state
from scratch, recovering after a loss, migrating to a new basis) is not an episode beside them, however exceptional its
trigger: record it as a **candidate constituent job**, or as a circumstance, until mapping tests it. Having several
episodes does not by itself show that a job can be mapped as one. Whether they hold together as one job is tested when the job is mapped: if its map
can be read as one coherent sequence (with episodes running through it), the job stands; if it needs several
independent cycles, each with its own beginning, end and outcomes, the job is really a higher-level job whose episodes
are **constituent jobs**, each mapped separately. Record that as an open question until the map settles it, and do not
use the step types to settle it in advance: that designs a workflow instead of finding the job.

## The other jobs

| Category | What it is | Test |
|---|---|---|
| **Main job** | The job being analysed: the one the map will be built for | Exactly one per topology |
| **Constituent job** | Part of the main job: one of its episodes found, in mapping, to need its own map | Same executor and intent as the main job; its result is part of the main job's |
| **Adjacent job** | A distinct job performed by the **same** executor | A **distinct desired outcome**: the executor is after a different result, not just doing something at a different time. Its own trigger, recipient and completion support that, but do not establish it (steps have those too). Otherwise it is a step or an episode |
| **Related job** | A job performed by **another** executor that touches the main job | Its executor is not the main executor; if it is, it is adjacent or constituent |

The categories carry the weight: whether a job is the main job, part of it, an independent job of the same executor,
or another executor's. How a job stands **in time** (*before*, *after*, *alongside*) is useful for an adjacent job, but
secondary; record it only where it helps.

A related job says **how it stands to the main job**:

| Relation | Meaning |
|---|---|
| **changes** | Alters the state the main job maintains or depends on; its result must be taken in (a transfer of shares, a share issue) |
| **enables** | Provides something the main job needs, without changing its subject |
| **constrains** | Sets limits on how the main job may be done |
| **governs** | Authorises, regulates or oversees it |
| **consumes** | Uses what the main job produces or maintains |
| **responds to** | Is set off by it |

### Which related jobs to include

Many executors touch any main job; a topology that lists them all stops being useful. **Include a related job when
its result changes, constrains, validates or materially depends on the main job's object, and understanding that
relationship is needed to establish the main job's boundary** (what it must take in, what it must provide, who may
decide what it holds). Leave out jobs that merely use the main job's result in passing, or touch it only through
another related job already listed.

- **Merge only what is the same job.** Executors are merged into one, with one related job, only when they pursue the
  same desired outcome, by the same rule as the main executor (*Unify when the desired outcome is the same*). Lenders,
  acquirers and advisers who each need to establish who holds the shares before relying on it pursue one outcome: one
  related job (*establish title before relying on it*), one executor (*relying party*). A transferor disposing of
  shares, a transferee acquiring them and a personal representative administering an estate stand in the same
  relationship to the main job (each changes who holds the shares) but pursue different outcomes: three related jobs.
  A shared relationship may be shown by grouping their rows together, never by merging their executors or jobs.
- **Record what was left out.** List related jobs considered and excluded in the main job's notes, with why, so the
  next reader does not add them back.

### Changing the world, and recording it

The commonest misplacement: a job that **changes the reality** (issuing shares, transferring them, buying them back)
put inside, or beside, the job that **maintains a representation** of that reality (the record of who owns them). They
are separate jobs, and usually separate executors, even when one person coordinates both. Decompose them:

| Job | Executor | Category |
|---|---|---|
| Authorise a share issue | Board | Related: governs |
| Carry out a share issue | The company, through its authorised officers | Related: changes |
| Take the resulting holdings into the record | Company secretary | An episode of the main job |

Then check the **direction of the seam**. Recording is not always passive: in some domains the act of recording gives
the change its legal effect (entry in a share register may complete a transfer). Where it does, say so: the main job
does not merely receive the change from the world, it takes part in making it. The seam then runs both ways, and the
job map will have an Execute step with consequences outside the record.

### Event-driven and periodic obligations

An obligation triggered by the same event as a piece of the main job's work (notifying a registry when a change is
made) is not part of that work just because it shares the trigger. Ask the outcome question: **is meeting the
obligation necessary to achieve the executor's desired outcome, or does it serve a distinct outcome** (keeping a
regulator's record current, say)? If necessary, it is a step of the episode, or of the related job that makes the
change; if distinct, it belongs to a separate job, which may be adjacent or part of a broader one (below). Which
events create an obligation at all, and with what deadlines, is a fact about the domain to be checked against its
sources, not assumed. Until both are settled, record the obligation in the framing as an open boundary question, not
as a rule (*changes may create notification obligations; whether a notification completes the change or belongs to a
separate reporting job is open*).

An obligation with **its own trigger and lifecycle** (an annual return) is a candidate job. Before calling it adjacent,
test its altitude: if its scope is wider than the main job's object (an annual return covers far more than share
ownership), it belongs to a broader job (*maintain the company's statutory information*), not beside the main job.
Then do not list it as an adjacent job: record a **boundary question** in the framing, saying where event-driven and
periodic obligations are handled, and leave the broader job to its own topology. Only an obligation whose scope is
the main job's object, with a lifecycle of its own, is adjacent.

**The statement must match the reason.** A candidate's statement and the signal that makes it distinct must describe
the same thing. A job stated as one activity (*report shareholding information*) but justified by another's lifecycle
(the annual return's cycle) is not yet a job: restate it as what actually has that lifecycle, then test that.

**Supplying another job is not a job by itself.** That the main job's record feeds another executor's job is captured
by that related job (*consumes*). It becomes an adjacent job of the main executor only when supplying pursues a
desired outcome of its own (satisfying a particular information need, where the main job preserves authoritative
information), not merely because information flows or each request has a start and end.

### Rules of method are not facts about the domain

The tests in this file decide how to classify what the evidence shows. A classification they produce (this obligation
is a step, these executors are one) is a **proposal about this domain**, held with the evidence behind it, not a
general truth about the domain. Do not write one into the topology as a domain assertion (*each change must be
notified; that notification completes it*) unless the evidence has established both the facts and the boundary. Where
it has not, state the facts as open and the classification as proposed. The same applies to feedback taken from a
review: apply it as a test, not as a conclusion.

### Naming a job from its executor's side

A job is named for what **its executor** is trying to get done, at a breadth that covers its variants. A job named for
an output (*Evidence a holding*, *Produce the report*) usually hides two jobs:

- the **consumer's** job (a shareholder establishing what they own at a given date), a related job with its own
  executor;
- the **supplier's** job (*provide authoritative information about share ownership*), which may be an adjacent job of
  the main executor, covering current and historical, routine and disputed requests alike.

Do not conflate them; their outcomes will differ.

### The intent and difference

For every job other than the main job, record its **core intent and how it differs from the main job's**: *what is*
against *what if*, a permanent record against an independent check, a standing state against a transaction. This is
the test that the job is genuinely distinct, and the first place a sub-domain boundary shows: a change of intent, time
horizon, lifecycle, authority or language between two jobs is a boundary signal. Record any as a hypothesis in the
framing; sub-domains are settled through the glossary's folders, not here.

Do not force everything discovered into the main job. The topology exists so that the main job keeps a coherent edge
while the wider domain stays on the page.

## Qualifiers and circumstances

Outcome-Driven Innovation also names **emotional** and **social** jobs. Keep the two apart:

- **emotional**: how the executor wants to feel, or avoid feeling (*avoid the anxiety of being blamed when a filing is
  late*);
- **social**: how the executor wants to be perceived by others (*be seen as a reliable custodian of the company's
  records*).

Record them as **qualifiers on the job**, never as jobs of their own; the job map turns them into outcomes on its steps.
Record one only where the evidence supports it. A topology with no qualifiers is fine; a qualifier invented to fill the
slot is not.

**Circumstances.** Situations in which the executor must do materially different things: first-time against routine,
contested against agreed, a listed company against a private one. Record them on the job. A circumstance that changes
the desired outcome, not just the steps or the scale, is a sign of a different job.

## The jobs left out

Two of Ulwick's categories are deliberately not part of a topology. **Consumption-chain jobs** (acquiring, learning,
using, getting help with a product) and **purchase-decision jobs** (the buyer's financial criteria) are about a
product, not the domain, and belong to product work. A reader arriving from the Ulwick literature should know they were
sent there, not forgotten.

## Framing

A few lines above the jobs:

- the **core executor** (by capacity) and the **main job**, in full;
- **execution seams**: what happens outside any system and what crosses back in, and in which direction, including
  where recording gives a change its effect;
- any **sub-domain split** already evident, stated as a hypothesis with the signal that prompted it;
- **boundary questions** left open (an obligation that may belong to a broader job; the breadth of the main job's
  object).

## Settle the topology before mapping

Three questions shape everything downstream; settle them, or record them as open, before the main job is mapped:

1. **Is the main job's object the right breadth?** (*Altitude and breadth*.)
2. **Is it one job, or a higher job with constituent jobs?** Recorded as open and tested by the map.
3. **Where does changing the world end and maintaining its representation begin?** (*Changing the world, and recording
   it*.)

## Errors to watch for

- **A title as an executor.** *Senior analyst* says where someone sits, not what they are getting done; *Company
  secretary* is fine as a name only if the capacity is stated.
- **Splitting on scale.** A listed company's registry treated as a different executor because it is bigger, when its
  desired outcome is the same.
- **A process as a job.** *Process the transfer form* names today's mechanism. Ask what the form is for.
- **A role's coordination as the role's job.** The secretary's work on a share issue recorded as a secretary's job.
- **Changing the world filed as an adjacent job.** *Carry out a change to share capital* as the company secretary's
  job, when it is a related job that changes what the main job records.
- **An episode as an adjacent job.** *Correct the register* listed beside the main job instead of on it.
- **A completing step as an adjacent job.** Notifying a registry of one change, listed as a job instead of as part of
  completing the change.
- **A broader job's obligation as an adjacent job.** A periodic obligation wider than the main job's object, listed
  beside it instead of recorded as a boundary question.
- **A statement that does not match its signal.** One activity stated, another's lifecycle used to justify it.
- **An undertaking among the episodes.** A recovery or rebuild with its own beginning and end, listed beside routine
  episodes.
- **A topology of everyone.** Related jobs added because an executor touches the main job, not because the
  relationship helps establish its boundary.
- **Executors merged by relationship.** Different executors folded into one because they stand to the main job the
  same way, though their desired outcomes differ.
- **An adjacent job on trigger alone.** A job separated because it has its own trigger or completion, with no distinct
  desired outcome.
- **A modelling choice stated as a domain rule.** A classification written as though the domain required it.
- **A job named for its output.** *Evidence a holding*, hiding the consumer's job and the supplier's.
- **A step promoted to an adjacent job.** *Obtain board approval* has no life outside the transaction it approves.
- **A related job swallowed into the main job.** The auditor's verification written as the main executor's Monitor
  step.
- **The main job at the wrong altitude or breadth.** Too low and the adjacent jobs are steps of a job nobody has
  stated; too high and the map will have forty steps; too narrow and edge cases need artificial distinctions.
- **An org chart wearing a topology.** One job per department, executors named by title, related jobs that are the
  reporting line.
- **A solution in the statement.** *Maintain the register in the system*: the last three words are the product.
- **A qualifier forced or mislabelled.** An emotional concern labelled social, or a qualifier nobody expressed.
- **Using the map to settle the topology.** Choosing the main job by which version gives a tidier sequence of step
  types.
