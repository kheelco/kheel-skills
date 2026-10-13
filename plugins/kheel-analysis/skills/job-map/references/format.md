# Format, rendering and where it lives

## The job map document

One Markdown document per job, in three parts: the job, the steps as a summary table, and a full entry for each step
that has more to say than its row (and for every step when the map is synced). An entry repeats what its row says and
adds the rest. Where a step has an entry, the entry is authoritative and the row summarises it; a row and an entry that
disagree are a defect.

````markdown
# Job map: Record a change to the membership roll

**Job:** Record a change to who belongs to the club or on what terms.
**Executor:** Membership secretary. A constituent job of
[Maintain the membership roll](../job-topology.md#maintain-the-membership-roll).

## Coherence

Progressions compared: taking in a change (a change, or a request for one, reaches the secretary; ends when the roll
states the position after it); checking the roll (a check falls due; ends with the extent of agreement established and
each discrepancy referred); correcting the roll (an error is found outside any change; ends with the roll restated and
the error still visible). Different beginnings, results and completions: three constituent jobs. This map is the
first; the others are mapped separately.

## Steps

| Type | Step | Outcomes |
|---|---|---|
| Define | **Determine what the change alters** | Minimise the time it takes to establish which memberships and terms a change alters<br>Minimise the likelihood that part of a change is missed (one member of a family membership) |
| Locate | **Obtain the evidence the change rests on**<br>*arrives from the world: the application, the resignation, the payment* | Minimise the time between a change and its evidence reaching the secretary<br>Minimise the likelihood that a change is taken up on incomplete evidence |
| Confirm | **[Confirm the change is authorised](#confirm-the-change-is-authorised)**<br>*arrives from the world: the committee's decision* | Minimise the likelihood that a change is entered without the authority it requires |
| Execute | **Enter the change in the roll** | Minimise the time between the conditions for entry being met and the change being entered<br>Minimise the likelihood that the position before the change can no longer be established |
| Modify | **Resolve an obstacle to completing the change** | Minimise the time it takes to establish whether a problem lies in this change or in an earlier entry (an earlier entry is handed on for correction) |
| Conclude | **Establish that the roll states the position after the change** | Minimise the likelihood that a change is left part-entered |

Types that yielded nothing: Prepare (nothing found; the figures are worked out under Define); Monitor (watching
pending changes happens across many changes, which suggests it belongs to the higher job).

## Entries

### Confirm the change is authorised

- **Type:** Confirm
- **Seam:** Arrives from the world: the committee's decision, where the club's rules require one.
- **Outcomes:**
  - Minimise the likelihood that a change is entered without the authority it requires.
- **Source:** Membership secretary interviews, 2026-03.
- **Notes:** Eligibility of the person (are they entitled to the grade?) is a separate question from authority, kept as
  its own outcomes or step if it proves distinct.
````

### The steps table

Three columns, steps in the order an executor would describe them:

| Column | Holds |
|---|---|
| **Type** | One of the eight step types. |
| **Step** | The step (verb + object, clarifier if needed) in bold, linked to its entry if it has one; then, on a new line (`<br>`), its seam in italics if it has one: *happens in the world: …* or *arrives from the world: …*. |
| **Outcomes** | One outcome per line (`<br>` between them), in the standard form. |

Before the table, a short **Coherence** paragraph: the principal progressions written in plain words, how they
compared (beginning, desired result, completion), and the conclusion: one job, or candidates mapped separately and
reported. After the table, a line listing the types that yielded nothing, and what each suggests about the boundary. A step is
identified by its statement within its map; restatements keep the old wording in its notes until citations are updated.

### The entries

`## Entries` holds a `###` section per step that has one, headed by its statement, in table order. Directly under the
heading comes its YAML block when synced. Then a bullet list, written `**Name:**`, leaving out what does not apply:
**Type**, **Seam**, **Outcomes** (a nested list, as in the row), **Episodes** (for a continuing job, which episodes pass through it: a diagnostic, not evidence that the job is one), **Order** (where the step runs alongside another or
repeats), **Source**, **Notes** (open questions start with *Open:*; candidates moved to the topology; survey results).

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
(`job-maps/record-a-change-to-the-membership-roll.md`). Ask if that is not evident.
