# Format, rendering and where it lives

## The job map document

One Markdown document per job, in three parts: the job, the steps as a summary table, and a full entry for each step
that has more to say than its row (and for every step when the map is synced). An entry repeats what its row says and
adds the rest. Where a step has an entry, the entry is authoritative and the row summarises it; a row and an entry that
disagree are a defect.

````markdown
# Job map: Maintain the membership roll

**Job:** Maintain an accurate, current record of who belongs to the club and on what terms, over the life of the club.
**Executor:** Membership secretary. From the [job topology](../job-topology.md#maintain-the-membership-roll).

**Pre-check:** Lifecycle map (the default). Taking in changes, checking the roll and correcting it serve one result,
an accurate, current roll; each passes through the stages it needs. Providing information about membership serves a
different result and stays an adjacent job.

## Circumstances

- **C1 Founding:** the first roll, with no existing record.
- **C2 Volume:** a national federation at volume, with online joining (an online form is an example, not the job).
- **C3 Contested:** membership disputed, or ordered corrected by a tribunal.
- **C4 Recovery:** the roll rebuilt after records are lost or found unreliable.

## Steps

| Type | Step | Outcomes |
|---|---|---|
| Define | **Determine what the roll must hold**<br>*C1: set up the first roll* | Minimise the likelihood that a grade or term the club's rules provide for is not established |
| Locate | **Obtain the evidence for each change to the roll**<br>*arrives from the world: the application, the resignation, the payment* | Minimise the time between a change and its evidence reaching the secretary<br>Minimise the likelihood that a change is taken up on incomplete evidence |
| Prepare | **[Work out what each change does to the roll](#work-out-what-each-change-does-to-the-roll)**<br>*edge cases: family membership* | Minimise the likelihood that part of a change is missed |
| Confirm | **[Confirm a change is authorised and the person entitled to it](#confirm-a-change-is-authorised-and-the-person-entitled-to-it)**<br>*arrives from the world: the committee's decision; C3; edge cases: junior member* | Minimise the likelihood that a change is entered without the authority it requires<br>Minimise the likelihood that someone is given a grade they are not entitled to |
| Execute | **Enter each change in the roll** | Minimise the time between the conditions for entry being met and the change being entered<br>Minimise the likelihood that the position before a change can no longer be established |
| Monitor | **Establish whether the roll still agrees with its sources**<br>*standard: consistency; C4* | Minimise the likelihood that a discrepancy goes unidentified<br>Minimise the likelihood that a difference in form is treated as a discrepancy |
| Modify | **[Put the roll right where it has drifted](#put-the-roll-right-where-it-has-drifted)**<br>*C3* | Minimise the time it takes to establish what the roll should say<br>Minimise the likelihood that a correction hides what the roll said before |
| Conclude | **Establish that the roll states the current position** | Minimise the likelihood that the roll is relied on while a change is part-entered |

(A real map would have ten to twenty steps; this example shows one or two per stage.)

## Entries

### Confirm a change is authorised and the person entitled to it

- **Type:** Confirm
- **Seam:** Arrives from the world: the committee's decision, where the club's rules require one.
- **Outcomes:**
  - Minimise the likelihood that a change is entered without the authority it requires.
  - Minimise the likelihood that someone is given a grade they are not entitled to.
- **Episodes:** Taking in a change; a correction that needs authority.
- **Circumstances:**
  - C3 (contested): confirm what the tribunal has decided before going further.
- **Edge cases:**
  - Junior member: confirm a parent or guardian has consented to the change.
- **Source:** Membership secretary interviews, 2026-03.

### Work out what each change does to the roll

- **Type:** Prepare
- **Covers:** the memberships, grades and terms a change touches, and the date it takes effect.
- **Outcomes:**
  - Minimise the likelihood that part of a change is missed.
- **Edge cases:**
  - Family membership: work out the change for every person the membership covers, not only the one who asked.
    Outcome: minimise the likelihood that a change reaches one member of a family membership and not the others.

### Put the roll right where it has drifted

- **Type:** Modify
- **Outcomes:**
  - Minimise the time it takes to establish what the roll should say.
  - Minimise the likelihood that a correction hides what the roll said before.
- **Episodes:** A discrepancy found by the check; an error ordered corrected by a tribunal (same step, another
  trigger; the tribunal is a related job).
- **Order:** After Monitor, or whenever an error is found; returns to Confirm where the correction needs authority.
````

### The steps table

Three columns, steps in the order an executor would describe them:

| Column | Holds |
|---|---|
| **Type** | One of the eight step types. |
| **Step** | The step (verb + object, clarifier if needed) in bold, linked to its entry if it has one; then, on a new line (`<br>`), its seam in italics if it has one (*happens in the world: …* or *arrives from the world: …*), followed by the circumstances that change it (*C3*) and the edge cases it has (*edge cases: joint holding*), named only; what each requires is in the entry. |
| **Outcomes** | One outcome per line (`<br>` between them), in the standard form. |

Before the table, a **Pre-check** line: the kind of map (lifecycle, the default; or a flowing map of one constituent
job, when asked for), and anything sent back to the topology. For a lifecycle map, a **Circumstances** section lists
the circumstances as contextual modifiers (C1, C2, …), and the steps they change say so after their seam (*C3*). After the table, a line listing the types that yielded nothing, and what each suggests about the boundary. A step is
identified by its statement within its map; restatements keep the old wording in its notes until citations are updated.

### The entries

`## Entries` holds a `###` section per step that has one, headed by its statement, in table order. Directly under the
heading comes its YAML block when synced. Then a bullet list, written `**Name:**`, leaving out what does not apply:
**Type**, **Covers** (what the step spans, where it spans several things), **Seam**, **Outcomes** (a nested list, as in the row), **Episodes** (for a continuing job, which episodes pass through the step), **Circumstances** and **Edge cases** (each a nested item `<case>: <what the step must accomplish in that case>`, with any outcome of its own; see [steps](steps.md), *Circumstances and edge cases*), **Order** (where the step runs alongside another or
repeats), **Source**, **Notes** (open questions start with *Open:*; parts sent back to the topology; survey results).

### Drafts

A draft has the same shape, kept apart from the agreed map (a `.draft.md` beside it, or the console). In a draft, each
step and each outcome ends with its status, `[attested]`, `[inferred]` or `[proposed]`, unless it matches the step's.
When the user agrees the map, its marks are removed and material doubt stays as open questions.

## Syncing

As for the topology: an unsynced map has no IDs; a synced one gives every step an entry with the external system's
`id`, `version` and `lastUpdated` in a YAML block under its heading. Outcomes travel with their step; where the
external system holds outcomes as records of their own, follow its sync mechanism for them. Never invent an id,
version or timestamp; check versions before pushing.

## Rendering

**Default to the console.** A map is one job, a handful of steps and their outcomes, read and argued with.

| Shape | Good for |
|---|---|
| **The steps table** | The standard shape, and what most people mean by "job map". |
| **The whole document** | Analysts and review; contested steps. |
| **A step strip** | The steps alone, in order, grouped under their types, for a workshop wall or a slide. |
| **An outcome list** | Outcomes numbered for an opportunity survey, statements unchanged. |

## Where it lives

In a `job-maps/` folder beside the domain's `job-topology.md`, one document per job, named after the job
(`job-maps/maintain-the-membership-roll.md`; a constituent job's map is named after it). Ask if that is not evident.
