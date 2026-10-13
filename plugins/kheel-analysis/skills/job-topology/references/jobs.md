# Executors and jobs

The examples below are drawn from several domains (a club's membership roll, a fleet of vehicles, an estate, a
conference, a clinic) to illustrate rules that hold in any domain. None of them is a fact about the domain being
analysed.

## The executor

Define the executor by their **capacity**: the responsibility they carry in getting the job done (*the person or
organisation responsible for the club's record of its members*), not a title, office, department, seniority or
persona. Give the executor a convenient **name** (*Membership secretary*), an agent term in the glossary, but do not let
the name assume a formal office the domain does not always have: many clubs appoint no membership secretary, and the
job is still done. Where no existing word fits and a name is coined for the capacity, its glossary entry says it names
a functional role, not a formal or statutory office, so readers do not take it for one.

- **Unify when the desired outcome is the same.** People getting the same job done, trying to achieve the same result,
  are one executor, however different their scale, volume, infrastructure, frequency, seniority or obligations. A
  volunteer secretary, a committee member doing it themselves and a paid administrator are one executor; so, at first,
  is a national federation's membership office, whose differences (volume, online joining, regulation) are
  **circumstances** of the same job.
- **Split only when the desired outcome changes.** Where the intent or the shape of the job is materially different, it
  is a different executor, and usually a different job. A treasurer forecasting next year's membership income is not
  the membership secretary at a higher level: the intent (*what if* against *what is*) and the lifecycle (throwaway
  against permanent) differ. More steps, more volume or different infrastructure are not reasons to split.

Record, for each executor, a line on what was unified or split and why.

## Roles are not jobs

An executor's role often spans several jobs, and coordinating someone else's job does not make it theirs. A practice
manager may chase a supplier, book the courier and sign for the delivery; that does not put the supplier's delivery in
the practice manager's job. Ask, of each thing the executor does: **is this getting their job done, or helping someone
else get theirs done?** Help given to another job is, at most, a step of the executor's own job (*confirm the delivery
has been authorised*) or a sign of a related job.

## The core functional job

State it as **verb + object + contextual clarifier**: *Maintain* an accurate, current *record of who belongs to the
club and on what terms* *over the life of the club*. The verb and object, without the clarifier, are the job's
**name**, which identifies it (*Maintain the membership roll*).

It must be free of any solution, independent of current technology, stable enough to outlive any process, stated from
the executor's perspective, and about something they are trying to accomplish.

It must be **neutral about sequence**: it should not assume whether a change in the world comes before, during or as a
consequence of the job, where that differs between circumstances. *Bring the record into line with a change* assumes
the change has already happened, which is false wherever making the entry is what gives the change effect; *record a
change* holds either way. The same applies to every job in the topology and every job map's heading.

A job whose result is **assurance** (to verify, check, validate, audit or reconcile something) must say which
**standard** it is after:

- **consistency**: the thing agrees with the evidence available for it (a roll that matches the payments received);
- **correctness**: the underlying state is as it should be (everyone on the roll is in fact entitled to be).

Agreement with sources does not establish correctness: sources can be missing, wrong, in conflict, or copied from the
record they are checked against. The two are different results, and may be different jobs. Name the standard in the
statement or its clarifier, and let the map follow it.

### Altitude and breadth

- **Would it still be the job under a completely different process?** If not, it is too low.
- **Does it have a beginning and an end, or a standing state with recurring work?** If neither (*run the club*), it is
  too high. If a standing state, see *Continuing jobs* below.
- **Is there one executor for it?** Two executors in one statement is usually two jobs.
- **Is the object the right breadth?** Test it against edge cases from the domain, cases at the edge of what the
  executor must keep coherent (for a membership roll: a family membership, an honorary member, a suspended member, a
  member moving between grades). If the executor cannot handle them without artificial distinctions, the object is too
  narrow (*who belongs* where *who belongs and on what terms* is meant). If widening it brings in several independent
  results, it is too broad. Record the cases tried and what they showed.

### Continuing jobs and their episodes

Some jobs have a beginning, execution and end (*settle an estate*, *run a conference*). Others are **continuing**: they
keep something in a desired state indefinitely (*keep the fleet roadworthy*, *maintain the membership roll*). A
continuing job is legitimate, and often the right main job, because its intent is the standing state, not any one
piece of work. It shows in the work the executor does when nothing new arrives: a fault found on inspection, a
discrepancy with old records, a dispute, a rebuild after loss, a question about the state at a past date.

A continuing job is done through **episodes**: recurring or exceptional executions of part of the job, each with a
trigger.

| Trigger | Example episode (membership roll) | Example episode (fleet) |
|---|---|---|
| **Event-driven**: something arrives | Take in a change to the roll | Deal with a reported fault |
| **Periodic**: a cycle comes round | Check the roll against its sources | Carry out a scheduled service |
| **Exceptional**: something is found wrong | Correct the roll | Withdraw a vehicle from use |

Episodes are **not separate jobs** while they share the main job's executor and intent; they are recorded on the main
job's entry, each with its trigger.

**Keep episodes at one altitude.** Episodes are the recurring or occasional modes of keeping the state, each a modest
piece of work. An exceptional undertaking big enough to have its own beginning, execution and end (rebuilding the state
from scratch, recovering after a loss, moving to a new basis or a new keeper) is not an episode beside them, however
exceptional its trigger: record it as a **candidate constituent job**, or as a circumstance, until mapping tests it.

Whether the episodes hold together as one job is tested by the job map's **coherence test**: do they share one
beginning, desired result and completion, as one progression? If so, the job stands; if they are several
progressions, the job is a higher-level job whose episodes are **constituent jobs**, each mapped separately. That a set
of steps can be found for every episode is not evidence either way. Treat a continuing main job as a **hypothesis** of
a single job until that test is run, record the question as open, and do not use the step types to settle it: that
designs a workflow instead of finding the job.

## The other jobs

| Category | What it is | Test |
|---|---|---|
| **Main job** | The job being analysed: the one the map will be built for | Exactly one per topology |
| **Constituent job** | Part of the main job: one of its episodes found, in mapping, to need its own map | Same executor as the main job; its result is part of the main job's |
| **Adjacent job** | A distinct job performed by the **same** executor | A **distinct desired outcome**: the executor is after a different result, not just doing something at a different time. Its own trigger, recipient and completion support that, but do not establish it (steps have those too). Otherwise it is a step or an episode |
| **Related job** | A job performed by **another** executor that touches the main job | Its executor is not the main executor; if it is, it is adjacent or constituent |

The categories carry the weight: whether a job is the main job, part of it, an independent job of the same executor,
or another executor's. How a job stands **in time** (*before*, *after*, *alongside*) is useful for an adjacent job, but
secondary; record it only where it helps.

A related job says **how it stands to the main job**:

| Relation | Meaning |
|---|---|
| **changes** | Alters the state the main job maintains or depends on; its result must be taken in (a member resigning, a vehicle being damaged) |
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
  same desired outcome, by the same rule as the main executor (*Unify when the desired outcome is the same*). An
  insurer, a competition organiser and a venue manager who each need to confirm someone is a member before relying on
  it pursue one outcome: one related job (*establish membership before relying on it*), one executor (*relying
  party*). A member resigning, an applicant joining and the executor of a deceased member's estate stand in the same
  relationship to the main job (each changes who is on the roll) but pursue different outcomes: three related jobs.
  A shared relationship may be shown by grouping their rows together, never by merging their executors or jobs.
- **Record what was left out.** List related jobs considered and excluded in the main job's notes, with why, so the
  next reader does not add them back.

### Changing the world, and recording it

The commonest misplacement: a job that **changes the reality** (admitting a member, repairing a vehicle, dispensing a
medicine) put inside, or beside, the job that **maintains a representation** of that reality (the roll, the fleet
log, the medication record). They are separate jobs, and usually separate executors, even when one person coordinates
both. Decompose them:

| Job | Executor | Category |
|---|---|---|
| Decide on an application for membership | Committee | Related: governs |
| Join the club | Applicant | Related: changes |
| Record the new membership | Membership secretary | An episode of the main job |

Then check the **direction of the seam**. Recording is not always passive: in some domains the act of recording gives
the change its effect (a membership that begins on entry in the roll; a title that passes on registration). Where it
does, say so: the main job does not merely receive the change from the world, it takes part in making it. The seam
then runs both ways, and the job map will have an Execute step with consequences outside the record. Whether recording
has that effect is a fact about the domain, to be checked against its sources.

### Event-driven and periodic obligations

An obligation triggered by the same event as a piece of the main job's work (notifying a federation when a member
joins) is not part of that work just because it shares the trigger. Ask the outcome question: **is meeting the
obligation necessary to achieve the executor's desired outcome, or does it serve a distinct outcome** (keeping another
body's record current, say)? If necessary, it is a step of the episode, or of the related job that makes the change;
if distinct, it belongs to a separate job, which may be adjacent or part of a broader one (below). Which events create
an obligation at all, and with what deadlines, is a fact about the domain to be checked against its sources, not
assumed. Until both are settled, record the obligation in the framing as an open boundary question, not as a rule
(*changes may create notification obligations; whether a notification completes the change or belongs to a separate
reporting job is open*).

An obligation with **its own trigger and lifecycle** (an annual return to a federation) is a candidate job. Before
calling it adjacent, test its altitude: if its scope is wider than the main job's object (the annual return covers
officers, finances and facilities as well as members), it belongs to a broader job (*maintain the club's standing with
its federation*), not beside the main job. Then do not list it as an adjacent job: record a **boundary question** in
the framing, saying where event-driven and periodic obligations are handled, and leave the broader job to its own
topology. Only an obligation whose scope is the main job's object, with a lifecycle of its own, is adjacent.

**The statement must match the reason.** A candidate's statement and the signal that makes it distinct must describe
the same thing. A job stated as one activity (*report membership numbers*) but justified by another's lifecycle (the
annual return's cycle) is not yet a job: restate it as what actually has that lifecycle, then test that.

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
an output (*Issue a membership card*, *Produce the report*) usually hides two jobs:

- the **consumer's** job (a member proving they belong, to enter a competition), a related job with its own executor;
- the **supplier's** job (*provide authoritative information about membership*), which may be an adjacent job of the
  main executor, covering current and historical, routine and disputed requests alike.

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

- **emotional**: how the executor wants to feel, or avoid feeling (*avoid the anxiety of being blamed when a member is
  wrongly turned away*);
- **social**: how the executor wants to be perceived by others (*be seen as a dependable keeper of the club's
  records*).

Record them as **qualifiers on the job**, never as jobs of their own; the job map turns them into outcomes on its steps.
Record one only where the evidence supports it. A topology with no qualifiers is fine; a qualifier invented to fill the
slot is not.

**Circumstances.** Situations in which the executor must do materially different things: first-time against routine,
contested against agreed, a large organisation against a small one. Record them on the job. A circumstance that
changes the desired outcome, not just the steps or the scale, is a sign of a different job.

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

- **A title as an executor.** *Senior analyst* says where someone sits, not what they are getting done; a title is fine
  as a name only if the capacity is stated.
- **Splitting on scale.** A large organisation's version of the job treated as a different executor because it is
  bigger, when its desired outcome is the same.
- **A process as a job.** *Process the application form* names today's mechanism. Ask what the form is for.
- **A role's coordination as the role's job.** Work done to help another's job recorded as the executor's own job.
- **Changing the world filed as an adjacent job.** A job that changes what the main job records listed as the main
  executor's own, instead of as a related job.
- **An episode as an adjacent job.** *Correct the record* listed beside the main job instead of on it.
- **A completing step as an adjacent job.** Notifying another body of one change, listed as a job instead of as part of
  completing the change.
- **A broader job's obligation as an adjacent job.** A periodic obligation wider than the main job's object, listed
  beside it instead of recorded as a boundary question.
- **A statement that does not match its signal.** One activity stated, another's lifecycle used to justify it.
- **A statement that assumes a sequence.** A job worded as following a change that, in some circumstances, it makes.
- **An assurance job with no standard.** *Verify the record* with no word on whether consistency or correctness is
  meant.
- **An undertaking among the episodes.** A recovery or rebuild with its own beginning and end, listed beside routine
  episodes.
- **A topology of everyone.** Related jobs added because an executor touches the main job, not because the
  relationship helps establish its boundary.
- **Executors merged by relationship.** Different executors folded into one because they stand to the main job the
  same way, though their desired outcomes differ.
- **An adjacent job on trigger alone.** A job separated because it has its own trigger or completion, with no distinct
  desired outcome.
- **A modelling choice stated as a domain rule.** A classification written as though the domain required it.
- **A job named for its output.** *Issue a membership card*, hiding the consumer's job and the supplier's.
- **A step promoted to an adjacent job.** *Obtain the committee's approval* has no life outside the change it
  approves.
- **A related job swallowed into the main job.** An auditor's verification written as the main executor's Monitor
  step.
- **The main job at the wrong altitude or breadth.** Too low and the adjacent jobs are steps of a job nobody has
  stated; too high and the map will have forty steps; too narrow and edge cases need artificial distinctions.
- **An org chart wearing a topology.** One job per department, executors named by title, related jobs that are the
  reporting line.
- **A solution in the statement.** *Maintain the roll in the system*: the last three words are the product.
- **A qualifier forced or mislabelled.** An emotional concern labelled social, or a qualifier nobody expressed.
- **Using the map to settle the topology.** Choosing the main job by which version gives a tidier sequence of step
  types.
