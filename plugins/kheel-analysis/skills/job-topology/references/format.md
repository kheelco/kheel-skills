# Format, rendering and where it lives

## The topology document

One Markdown document per domain, in four parts: the framing, the executors, the jobs as a summary table, and a full
entry for each job that has more to say than its row (and for every job when the topology is synced). An entry repeats
what its row says and adds the rest, so a reader has the whole job in one place. Where a job has an entry, the entry is
authoritative and the row summarises it; a row and an entry that disagree are a defect.

````markdown
# Membership roll job topology

The **membership secretary**, the person or organisation responsible for the club's record of its members, maintains
an accurate, current record of who belongs to the club and on what terms, over the life of the club.

Execution seams: applicants join, members resign and subscriptions are paid outside the roll; each arrives at the
roll to be taken in. Where the club's rules say membership begins on entry in the roll, the seam runs both ways:
recording takes part in making the change (unverified for this club).

Sub-domain hypothesis: the roll (what is) and membership planning (what if) differ in intent and lifecycle.

Boundary questions: whether the object covers people who are not members but have rights at the club (guests,
reciprocal members); whether notices to the federation complete a change or belong to a separate reporting job.

## Executors

| Executor | Capacity | Unified or split |
|---|---|---|
| **Membership secretary** | The person or organisation responsible for the club's record of its members (a functional role; many clubs appoint no one to it) | Unified: a volunteer secretary, a committee member doing it themselves and a paid administrator; a national federation's office at first too, its differences being circumstances |
| **Committee** | Decides on applications and on changes to membership terms | |
| **Applicant** | Seeks to join the club | |
| **Relying party** | Needs to confirm someone's membership before relying on it (an insurer, a competition organiser, a venue) | |
| **Treasurer** | Forecasts the club's membership income | Split from the membership secretary: the desired outcome is a forecast (*what if*), not the record (*what is*) |

## Jobs

| Job | Category | Executor | Intent and difference from the main job |
|---|---|---|---|
| **[Maintain the membership roll](#maintain-the-membership-roll)**<br>an accurate, current record of who belongs to the club and on what terms, over the life of the club | Main | Membership secretary | |
| **Provide authoritative information about membership** | Adjacent | Membership secretary | Satisfies a particular information need, current or historical, routine or disputed, where the main job preserves the information. Signal: intent. |
| **Decide on an application** | Related: governs | Committee | A decision on whether, and on what terms, someone joins. Signal: authority. |
| **Join the club** | Related: changes | Applicant | The applicant's own undertaking; the roll takes its result in. Signal: changing the world against representing it. |
| **Establish membership before relying on it** | Related: consumes | Relying party | Confidence at a date that someone belongs, for the relying party's own purpose. Signal: intent. |
| **Forecast membership income** | Related: consumes | Treasurer | *What if* against *what is*; works on forecasts that are thrown away. Signal: lifecycle. |

## Entries

### Maintain the membership roll

- **Statement:** Maintain an accurate, current record of who belongs to the club and on what terms, over the life of
  the club.
- **Category:** Main
- **Executor:** Membership secretary
- **Episodes:**
  - Take in a change to the roll (event-driven: a member joins, resigns, changes grade or particulars).
  - Check the roll against its sources (periodic).
  - Correct the roll (exceptional: an error found, a dispute).
- **Candidate constituent jobs:** Rebuild the roll (after records are lost or found unreliable).
- **Edge cases:** A family membership (several people, one subscription) and a move between grades (same person,
  different terms) break an object of *who belongs* alone; supports *who belongs and on what terms*.
- **Qualifiers:** Avoid the anxiety of being blamed when a member is wrongly turned away (emotional).
- **Circumstances:** The first roll when the club is founded; a national federation at volume, with online joining.
- **Map:** [Job map](job-maps/record-a-change-to-the-membership-roll.md)
- **Source:** Membership secretary interviews, 2026-03.
- **Notes:** Open: whether the episodes hold together as one job, or are constituent jobs of a higher one; to be tested
  by the map. Left out: the club's insurer setting premiums (touches the roll only through *Establish membership*).
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
### Maintain the membership roll

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
