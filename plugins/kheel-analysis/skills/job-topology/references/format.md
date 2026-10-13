# Format, rendering and where it lives

## The topology document

One Markdown document per domain, in four parts: the framing, the executors, the jobs as a summary table, and a full
entry for each job that has more to say than its row (and for every job when the topology is synced). An entry repeats
what its row says and adds the rest, so a reader has the whole job in one place. Where a job has an entry, the entry is
authoritative and the row summarises it; a row and an entry that disagree are a defect.

````markdown
# Share register job topology

The **company secretary** maintains an accurate, legally compliant record of who owns the company's shares over the
life of the company. Execution seams: share transfers are agreed and paid for between the parties, outside any
register; the register receives the signed transfer. Sub-domain hypothesis: the register (what is) and capital
planning (what if) differ in intent and lifecycle.

## Executors

| Executor | Capacity | Unified or split |
|---|---|---|
| **Company secretary** | Keeps the company's statutory records and filings | Unified: the in-house secretary and an outsourced provider do the same job |
| **Auditor** | Independently verifies the company's records | |
| **Chief financial officer** | Plans the company's capital structure | Split from the company secretary: intent is *what if*, not *what is* |

## Jobs

| Job | Category | Executor | Intent and difference from the main job |
|---|---|---|---|
| **[Maintain the record of share ownership](#maintain-the-record-of-share-ownership)**<br>an accurate, legally compliant record of who owns the company's shares over the life of the company | Main | Company secretary | |
| **Issue shares** | Adjacent: before | Company secretary | Creates new holdings under a resolution; a transaction with its own lifecycle, which the record then reflects. |
| **Verify the share register** | Related: governs | Auditor | Independent assurance that the record is right, at a point in time. |
| **Plan a capital raising** | Related: consumes | Chief financial officer | *What if* against *what is*; works on forecasts that are thrown away. |

## Entries

### Maintain the record of share ownership

- **Statement:** Maintain an accurate, legally compliant record of who owns the company's shares over the life of the
  company.
- **Category:** Main
- **Executor:** Company secretary
- **Qualifiers:** Not be the one held responsible when a filing is wrong or late (social).
- **Circumstances:** A first registration on incorporation, against routine changes.
- **Map:** [Job map](job-maps/maintain-the-record-of-share-ownership.md)
- **Source:** Company secretary interviews, 2026-03.
````

### The executors table

One row per executor: the executor's word in bold (an agent term in the glossary), their capacity in executing the job,
and what was unified or split and why.

### The jobs table

Four columns, the main job first, then adjacent and then related jobs:

| Column | Holds |
|---|---|
| **Job** | The job's name (verb + object) in bold, linked to its entry if it has one; then, on a new line (`<br>`), its contextual clarifier where it has one. |
| **Category** | `Main`, `Adjacent: <before / after / alongside>` or `Related: <enables / constrains / consumes / governs / responds to>`. |
| **Executor** | The executor's word, as in the executors table. |
| **Intent and difference from the main job** | Its core intent and how it differs, naming the signal (intent, time horizon, lifecycle, authority, language). Empty for the main job. |

A job is identified by its name; renames keep the old name in its notes until citations are updated. A table cell
cannot contain `|` or a line break other than `<br>`.

### The entries

`## Entries` holds a `###` section per job that has one, headed by its name, in table order. Directly under the
heading comes its YAML block when synced (see *Syncing*). Then a bullet list, written `**Name:**`, leaving out what
does not apply:

- **Statement**, **Category**, **Executor** and **Intent and difference**: as the row says.
- **Qualifiers**: emotional and social, each labelled.
- **Circumstances**: each, with what changes in it.
- **Seams**: where this job's execution leaves any system, if the framing does not already say.
- **Map**: a link to its job map, if it has one.
- **Source**, and **Notes** (open questions start with *Open:*; candidates rejected as steps; executor questions).

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
| **A diagram** | The main job in the centre, adjacent jobs around it labelled *before*, *after*, *alongside*, related jobs outside with their executors and relations. Derived from the document, never drawn separately (Mermaid `flowchart` unless the project uses another). |
| **Part of a domain analysis** | Framing and topology first, ahead of the job maps. |

## Where it lives

In the folder that stands for the domain, beside its glossary (`job-topology.md`), with its job maps in a `job-maps/`
folder beside it, one per job. Ask if that is not evident. A synced topology is pushed and pulled as *Syncing* says.
