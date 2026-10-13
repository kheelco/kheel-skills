# Format, rendering and where it lives

## The job map document

One Markdown document per job, in three parts: the job, the steps as a summary table, and a full entry for each step
that has more to say than its row (and for every step when the map is synced). An entry repeats what its row says and
adds the rest. Where a step has an entry, the entry is authoritative and the row summarises it; a row and an entry that
disagree are a defect.

````markdown
# Job map: Maintain the record of share ownership

**Job:** Maintain an accurate, legally compliant record of who owns the company's shares over the life of the company.
**Executor:** Company secretary. From the [job topology](../job-topology.md#maintain-the-record-of-share-ownership).

## Steps

| Type | Step | Outcomes |
|---|---|---|
| Define | **Determine what change to ownership must be recorded** | Minimise the time it takes to establish what a transfer changes<br>Minimise the likelihood that a change affecting several share classes is recorded as one |
| Confirm | **[Confirm that the transfer is permitted](#confirm-that-the-transfer-is-permitted)**<br>*arrives from the world: the board's approval* | Minimise the likelihood that a transfer breaching a pre-emptive right is recorded<br>Minimise the time it takes to establish which restrictions apply |
| Execute | **Record the completed transfer** | Increase the likelihood that a transfer is recorded on the day it takes effect |
| Conclude | **Notify the holders of the change** | Minimise the likelihood that a holder is not told of a change to their holding |

Types that yielded nothing: Locate, Prepare, Monitor, Modify (not yet asked; see notes).

## Entries

### Confirm that the transfer is permitted

- **Type:** Confirm
- **Seam:** Arrives from the world: the board's approval of the transfer, where the constitution requires it.
- **Outcomes:**
  - Minimise the likelihood that a transfer breaching a pre-emptive right is recorded.
  - Minimise the time it takes to establish which restrictions apply.
- **Source:** Company secretary interviews, 2026-03.
- **Notes:** Open: whether the secretary or the board decides that a restriction applies; if the board, this may be
  part of a related job.
````

### The steps table

Three columns, steps in the order an executor would describe them:

| Column | Holds |
|---|---|
| **Type** | One of the eight step types. |
| **Step** | The step (verb + object, clarifier if needed) in bold, linked to its entry if it has one; then, on a new line (`<br>`), its seam in italics if it has one: *happens in the world: …* or *arrives from the world: …*. |
| **Outcomes** | One outcome per line (`<br>` between them), in the standard form. |

After the table, a line listing the types that yielded nothing, and why (none found, or not yet asked). A step is
identified by its statement within its map; restatements keep the old wording in its notes until citations are updated.

### The entries

`## Entries` holds a `###` section per step that has one, headed by its statement, in table order. Directly under the
heading comes its YAML block when synced. Then a bullet list, written `**Name:**`, leaving out what does not apply:
**Type**, **Seam**, **Outcomes** (a nested list, as in the row), **Order** (where the step runs alongside another or
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
(`job-maps/maintain-the-record-of-share-ownership.md`). Ask if that is not evident.
