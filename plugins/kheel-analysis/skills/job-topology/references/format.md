# Format, rendering and where it lives

## The topology document

One Markdown document per domain, in four parts: the framing, the executors, the jobs as a summary table, and a full
entry for each job that has more to say than its row (and for every job when the topology is synced). An entry repeats
what its row says and adds the rest, so a reader has the whole job in one place. Where a job has an entry, the entry is
authoritative and the row summarises it; a row and an entry that disagree are a defect.

````markdown
# Share register job topology

The **company secretary**, the person or organisation responsible for the company's record of share ownership,
maintains an accurate, legally compliant record of who owns the company's shares over the life of the company.

Execution seams: transfers are agreed, signed and paid for between the parties, and shares are issued under the
company's authority, outside the record; both arrive at the record to be taken in. Where entry in the register is what
gives a transfer effect, the seam runs both ways: recording takes part in making the change.

Sub-domain hypothesis: the record (what is) and capital planning (what if) differ in intent and lifecycle.

Boundary questions: whether the object is *share ownership* or *share capital and its ownership* (tried against a
subdivision and a conversion between classes; not yet settled); whether periodic statutory reporting belongs to a
broader job of maintaining the company's statutory information.

## Executors

| Executor | Capacity | Unified or split |
|---|---|---|
| **Company secretary** | The person or organisation responsible for the company's record of share ownership | Unified: an appointed secretary, a director doing it themselves and an outsourced provider; a listed company's registry at first too, its differences being circumstances |
| **Board** | Decides on changes to the company's share capital | |
| **Company** | Carries out changes to its share capital, through its authorised officers | |
| **Auditor** | Independently verifies the company's records | |
| **Chief financial officer** | Plans the company's capital structure | Split from the company secretary: the desired outcome is a plan (*what if*), not the record (*what is*) |

## Jobs

| Job | Category | Executor | Intent and difference from the main job |
|---|---|---|---|
| **[Maintain the record of share ownership](#maintain-the-record-of-share-ownership)**<br>an accurate, legally compliant record of who owns the company's shares over the life of the company | Main | Company secretary | |
| **Provide authoritative information about share ownership** | Adjacent | Company secretary | Answers a request, current or historical, routine or disputed, with its own lifecycle; reader-facing rather than keeping the record. Signal: intent. |
| **Carry out a share issue** | Related: changes | Company | Changes the company's capital and who owns it; the record then takes the result in. Signal: changing the world against representing it. |
| **Authorise a share issue** | Related: governs | Board | A decision on whether, and on what terms, shares are issued. Signal: authority. |
| **Verify the share register** | Related: governs | Auditor | Independent assurance that the record is right, at a point in time. Signal: authority. |
| **Plan a capital raising** | Related: consumes | Chief financial officer | *What if* against *what is*; works on forecasts that are thrown away. Signal: lifecycle. |

## Entries

### Maintain the record of share ownership

- **Statement:** Maintain an accurate, legally compliant record of who owns the company's shares over the life of the
  company.
- **Category:** Main
- **Executor:** Company secretary
- **Episodes:**
  - Incorporate a change in share ownership (event-driven: a transfer, an issue or a transmission arrives).
  - Verify the accuracy of recorded ownership (periodic).
  - Correct an ownership record (exceptional: an error or a dispute).
- **Qualifiers:** Avoid the anxiety of being blamed when a deal is held up by the record (emotional).
- **Circumstances:** A first registration on incorporation; a listed company's registry, at volume and with settlement.
- **Map:** [Job map](job-maps/maintain-the-record-of-share-ownership.md)
- **Source:** Company secretary interviews, 2026-03.
- **Notes:** Open: whether the episodes hold together as one job, or are constituent jobs of a higher one; to be tested
  by the map.
````

### The framing

A few paragraphs, as [jobs](jobs.md) (*Framing*) describes: the core executor by capacity and the main job in full;
execution seams and their direction; sub-domain hypotheses; boundary questions left open.

### The executors table

One row per executor: the executor's name in bold (an agent term in the glossary), their capacity (the responsibility
they carry), and what was unified or split and why.

### The jobs table

Four columns, the main job first, then constituent, adjacent and related jobs:

| Column | Holds |
|---|---|
| **Job** | The job's name (verb + object) in bold, linked to its entry if it has one; then, on a new line (`<br>`), its contextual clarifier where it has one. |
| **Category** | `Main`; `Constituent`; `Adjacent`, optionally with its place in time (`Adjacent: before`, `after`, `alongside`); or `Related: <changes / enables / constrains / governs / consumes / responds to>`. |
| **Executor** | The executor's name, as in the executors table. |
| **Intent and difference from the main job** | Its core intent and how it differs, naming the signal (intent, time horizon, lifecycle, authority, language). Empty for the main job. |

Episodes are not rows: they are listed on the main job's entry. A job is identified by its name; renames keep the old
name in its notes until citations are updated. A table cell cannot contain `|` or a line break other than `<br>`.

### The entries

`## Entries` holds a `###` section per job that has one, headed by its name, in table order. Directly under the
heading comes its YAML block when synced (see *Syncing*). Then a bullet list, written `**Name:**`, leaving out what
does not apply:

- **Statement**, **Category**, **Executor** and **Intent and difference**: as the row says.
- **Episodes** (a continuing job): each with its trigger, event-driven, periodic or exceptional; and, separately,
  any **candidate constituent jobs** (undertakings too large to be episodes), until mapping tests them.
- **Edge cases**: the cases the object's breadth was tested against, and what they showed.
- **Qualifiers**: emotional and social, each labelled, only where evidence supports them.
- **Circumstances**: each, with what changes in it.
- **Seams**: where this job's execution leaves any system, and in which direction, if the framing does not already
  say.
- **Map**: a link to its job map, if it has one.
- **Source**, and **Notes** (open questions start with *Open:*; candidates rejected as steps or episodes; related
  jobs considered and left out, with why, on the main job; executor questions).

### Drafts

A draft has the same shape, kept apart from the agreed topology (`job-topology.draft.md`, or the console). In a draft,
each job's name ends with its status, `[attested]`, `[inferred]` or `[proposed]`, and any other claim (an executor, a
category, a relation) whose status differs ends with its own mark. When the user agrees jobs into the topology they
move across without their marks; material doubt stays as an open question.

## Syncing

A topology that is not synced has no IDs. Only when it is synced with an external system does each job carry the
system's `id`, `version` and `lastUpdated` (its last-modified time or ETag), in a YAML block directly under the job's
entry heading:

````markdown
### Maintain the record of share ownership

```yaml
id: 51c0e2
version: 3
lastUpdated: 2026-10-02T04:11:09Z
```

- **Statement:** …
````

Every job of a synced topology has an entry. Where the sync mechanism prescribes another shape, follow it; where a
platform skill for it is available (for example `page-sync`), it says how a push and a pull go. Never invent an id,
version or timestamp; before pushing, check each job's version against the source.

## Rendering

**Default to the console.** A topology is short and almost always wanted for argument rather than filing.

| Shape | Good for |
|---|---|
| **Framing and the jobs table** | The standard shape. |
| **The whole document** | Analysts and review; contested executors or jobs. |
| **A diagram** | The main job in the centre with its episodes or constituent jobs inside it, adjacent jobs beside it, related jobs outside with their executors and relations. Derived from the document, never drawn separately (Mermaid `flowchart` unless the project uses another). |
| **Part of a domain analysis** | Framing and topology first, ahead of the job maps. |

## Where it lives

In the folder that stands for the domain, beside its glossary (`job-topology.md`), with its job maps in a `job-maps/`
folder beside it, one per job. Ask if that is not evident. A synced topology is pushed and pulled as *Syncing* says.
