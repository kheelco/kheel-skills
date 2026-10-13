# Desired outcomes

For each significant step, the executor has a way of judging whether it went well. Desired outcomes make that judgement
explicit as **measurable qualities of successful execution**, not restatements of the step.

## The statement

**Direction + measure + object of control + contextual clarifier:**

> **Minimise the time** it takes to *determine whether a newly identified obligation applies*.
> **Minimise the likelihood** that *an applicable obligation is overlooked*.
> **Minimise the likelihood** that *an obligation is wrongly treated as applicable*.
> **Minimise the variability** in *how a fault's severity is judged from one inspector to another*.
> **Increase the likelihood** that *a change is recorded on the day it takes effect*.

*Minimise the time*, *minimise the likelihood*, *minimise the variability* and *increase the likelihood* cover nearly
everything; *minimise the number* (a count: properties viewed, reports paid for) is allowed where a count is what the
executor judges by. *Minimise the effort* is allowed, but effort is harder to measure than time or likelihood: where it can be
restated as one of them (the time spent, the number of times the executor has to go back), do so, and otherwise note
that its measure needs settling when the outcomes are validated with practitioners. An outcome that needs another
opening is worth a second look.

A step usually carries two to four outcomes once they have been researched. Harvest them from what goes wrong today:
what takes too long, the mistake that recurs, the result that varies from person to person. Write the object in glossary nouns, and keep each outcome
attached to its step; outcomes are never pooled across a map.

**Tensions are recorded, not resolved.** Outcomes on a step may pull against each other (not overpaying, and not
losing the property to a competing offer). Record both as the executor states them, and note the tension; do not
choose between them, or reword one to favour a strategy. Which matters more is for executors to say, through
validation and the opportunity survey, not for the analyst to optimise. Watch for an outcome that **encodes a
decision strategy** (*… that a property the purchaser would have paid more for is lost*): it may be legitimate, but
mark it for validation.

**Qualifiers become outcomes.** The emotional and social qualifiers recorded on the job in the topology yield outcomes
on the steps they bear on, in the same form: *minimise the likelihood that a late filing is attributed to the executor*.

## Two kinds of completeness

Keep two questions apart, and review them separately:

- **Functional completeness**: has the map found the work that must be accomplished? That is the steps' question
  ([steps](steps.md), *Coverage across circumstances*).
- **Outcome completeness**: has the map found the ways the executor measures each step's success?

A step is sound even while its outcomes are incomplete, and finding another outcome does not mean another step is
needed. Initial mapping records the outcomes the evidence offers; it need not discover them exhaustively. Outcomes are
refined with practitioners, through interviews and iteration, and their completeness is judged then.

## What an outcome is not

Not a feature, a requirement, an acceptance criterion, a KPI, a business objective, a benefit or a definition of done.
The test: **is it a quality of the step's execution the executor would recognise as their own standard, and could it
be measured?**

- *Minimise the time it takes to issue a membership card* is an outcome.
- *Cards are generated automatically* is a feature.
- *Ninety per cent of cards issued within a day* is a KPI: a target set on an outcome, a later act.
- *Record the transaction accurately* is the step with an adverb. Ask what *accurately* would be measured by.

## Checking each outcome

First, a quick check of the wording:

- **Measurable**: could it be measured, as time, likelihood, variability or a count?
- **Solution-independent**: does it hold whatever the means of doing the step?
- **A result, not a method**: does it say what the executor wants, rather than how to get it?
- **Specific**: are its object and context specific enough that two people would measure the same thing?
- **Distinct**: does it say something the step's other outcomes do not?

Then six deeper questions:

1. **Does it measure success, or specify a solution?** *Minimise the likelihood that a category is not provided for in
   the record* reads as a requirement on how the record is built. Restate it as the executor's judgement of the step
   (*… that a characteristic that must be kept is not established*).
2. **Which of its nouns are the domain's, and which are an implementation's?** Some concepts are unavoidable because
   they are part of the job's object (where the record is itself what the domain requires, its entries may be). Others
   assume a solution (a database row, a workflow state). Keep the first, and restate around the second.
3. **Is it within the executor's capacity, given how the domain works?** An outcome measures something the
   executor's execution can affect: within the responsibility their capacity carries, and consistent with the
   domain's causal rules (who decides what, what makes a change take effect, what evidence exists and who holds it).
   Check those rules against the glossary and the business rules, not assumption. Where the committee decides
   admissions, *minimise the likelihood that someone is admitted who should not be* belongs to the committee's job;
   the secretary's outcome is *minimise the likelihood that an admission is entered without the committee's
   decision*. Where entry in the roll is what makes membership begin, an outcome about the timing of membership is
   the secretary's after all: the causal rule decides whose outcome it is.
   *Minimise the likelihood that a change is made without the executor learning of it* may be beyond them; *minimise
   the time between a change and its evidence reaching them* is not. Likewise, work handed to another executor is not the
   job's to resolve: where a dispute goes to a tribunal, the job can minimise the likelihood that it goes
   unidentified, undocumented or unreferred, not that it goes unresolved.
4. **Does a time outcome have a measure?** *Within the time it must be* depends on a deadline that may not exist.
   Measure the time from the conditions being met to the step being done; record a statutory deadline separately, as a
   rule, once its source is checked.
5. **Is it an invariant in disguise?** A rule that must always hold (totals that must agree, a balance that must not go
   negative) is domain knowledge, and belongs to the glossary's rules or the business rules. It is a useful input to an
   outcome, not an outcome: the outcome is about the executor's execution, *minimise the likelihood that a change is
   completed in a way that leaves the totals in disagreement*, not *minimise the likelihood that the totals disagree*.
6. **Does it measure this job's success, or another job's?** *Minimise the likelihood that a member is unaware of a
   change to their membership* measures communicating with members. Unless that result is necessary to this job's desired
   result, the outcome, and often the step it sits on, belongs to another job: note it and send it to the topology.

## The opportunity survey

Outcomes written this way can be prioritised by surveying executors on each outcome's **importance** and their
**satisfaction** with how it is met today; the standard opportunity score is
*importance + max(importance − satisfaction, 0)*, and outcomes that score high are important and underserved. That
survey is quantitative research built on a finished map, not part of mapping. If one is run:

- keep the statements exactly as mapped, and number them for the survey only;
- screen respondents to the job's executor;
- read *underserved*, *appropriately served* and *overserved* off the scores, never assign them by judgement;
- record the results against the outcomes in their notes, with the survey's date and sample.

## Errors to watch for

- **Trade-offs resolved by the analyst.** Outcomes in tension reworded or dropped so one wins, or an outcome that
  encodes a decision strategy presented as settled.
- **Completeness conflated.** A step questioned because its outcomes are incomplete, or a step added because a new
  outcome was found.
- **Outcomes duplicated.** Two outcomes on one step that measure the same thing in different words.
- **Outcomes that restate the step.**
- **Outcomes that are features**: anything that names a mechanism, or could be shipped.
- **Outcomes that are targets**: a number in it is a KPI.
- **Outcomes pooled at the end of the map** instead of attached to their step.
- **Outcomes nobody said**: reasoned into being by the agent and marked attested.
- **Outcomes that are design requirements**: a quality of the solution, not of the executor's progress.
- **Another job's outcomes**: success measured for a result this job does not pursue.
- **Outcomes out of reach**: measuring what the executor cannot affect, given their capacity and the domain's causal
  rules (another party's decision, an effect the executor's act does not cause), or the resolution of work handed on.
- **Deadlines with no measure**: *within the time it must be*, with no deadline established.
- **Invariants as outcomes**: a rule about the state, not a measure of the executor's execution.
- **Effort with no measure**: *minimise the effort* where time or likelihood would say it more precisely.
