# Format, rendering and where it lives

## The topology document

One Markdown document per domain, in four parts: the framing, the executors, the jobs as a summary table, and a full
entry for each job that has more to say than its row (and for every job when the topology is synced). An entry repeats
what its row says and adds the rest, so a reader has the whole job in one place. Where a job has an entry, the entry is
authoritative and the row summarises it; a row and an entry that disagree are a defect.

````markdown
# Membership roll job topology

The **membership secretary**, the person or organisation responsible for the club's record of its members, maintains
the record of who belongs to the club and on what terms, over the life of the club.

Flags for deeper analysis: applicants join, members resign and subscriptions are paid outside the roll, and arrive
at it to be taken in; the club's rules may make membership begin on entry in the roll (unverified), in which case
recording takes part in making the change. Notices to the federation: whether one completes a change or belongs to a
separate reporting job.

Sub-domain hypothesis: the roll (what is) and membership planning (what if) differ in intent and lifecycle.

Boundary questions: whether the object covers people who are not members but have rights at the club (guests,
reciprocal members).

## Executors

| Executor | Capacity | Unified or split |
|---|---|---|
| **Membership secretary** | The person or organisation responsible for the club's record of its members (a functional role; many clubs appoint no one to it) | Unified: a volunteer secretary, a committee member doing it themselves and a paid administrator; a national federation's office at first too, its differences being circumstances |
| **Committee** | Decides on applications and on changes to membership terms | |
| **Applicant** | Seeks to join the club | |
| **Relying party** | Needs to confirm someone's membership before relying on it (an insurer, a competition organiser, a venue) | |
| **Treasurer** | Forecasts the club's membership income | Split from the membership secretary: the desired outcome is a forecast (*what if*), not the record (*what is*) |

## Jobs

| Job | Category | Executor | How it stands to the main job, and how its intent differs |
|---|---|---|---|
| **[Maintain the membership roll](#maintain-the-membership-roll)**<br>the record of who belongs to the club and on what terms, over the life of the club | Main | Membership secretary | |
| **Provide authoritative information about membership** | Related | Membership secretary | Satisfies a particular information need, current or historical, routine or disputed, where the main job preserves the information. Signal: intent. |
| **Decide on an application** | Stakeholder | Committee | Decides whether, and on what terms, someone joins, before the change is recorded. Signal: authority. |
| **Join the club** | Stakeholder | Applicant | The applicant's own undertaking; the roll takes its result in. Signal: changing the world against representing it. |
| **Establish membership before relying on it** | Stakeholder | Relying party | Uses the roll to confirm someone belongs, for its own purpose. Signal: intent. |
| **Forecast membership income** | Stakeholder | Treasurer | Uses the roll's numbers to forecast; *what if* against *what is*. Signal: lifecycle. |

## Entries

### Maintain the membership roll

- **Statement:** Maintain the record of who belongs to the club and on what terms, over the life of the club.
- **Category:** Main
- **Executor:** Membership secretary
- **Scope:** Members of every grade, past and present, and the terms each holds or held. Not guests or reciprocal
  members (open: see the framing).
- **Success criteria:** Accurate and current: everyone entitled to be on the roll is on it, on the right terms, and
  no one else (standard: correctness).
- **Edge cases:** A family membership (several people, one subscription) and a move between grades (same person,
  different terms) break an object of *who belongs* alone; supports *who belongs and on what terms*.
- **Qualifiers:** Avoid the anxiety of being blamed when a member is wrongly turned away (emotional).
- **Circumstances:** The first roll when the club is founded; a national federation at volume, with online joining.
- **Constituents:**

  | Candidate | Set off by | What was noticed | Lean | Status |
  |---|---|---|---|---|
  | Take in a change to the roll | A member joins, resigns, changes grade or particulars | Only happens when a change arrives; its result is the roll's | Likely an episode | Covered: Locate to Execute; separately mappable (not mapped yet) |
  | Check the roll against its sources | The annual check falls due | Done when nothing has changed; its own completion | Unclear | Covered: Monitor |
  | Correct the roll | An error is found, by the secretary or ordered by a tribunal | Sometimes inside a change, sometimes long after | Unclear | Covered: Modify |
  | Establish an authoritative roll | The club is founded, or records are lost | Rare, substantial, own beginning and end | Possibly a job of its own | Unresolved: not examined; the map's coverage test found a gap under recovery |
- **Map:** [Job map](job-maps/maintain-the-membership-roll.md)
- **Source:** Membership secretary interviews, 2026-03.
- **Notes:** Left out: the club's insurer setting premiums (touches the roll only through *Establish membership*).
````

### The framing

A few paragraphs, as [jobs](jobs.md) (*Framing*) describes: the core executor by capacity and the main job in full;
flags for deeper analysis (seams, obligations, supplying); sub-domain hypotheses; boundary questions left open.

### The executors table

One row per executor: the executor's name in bold (an agent term in the glossary), their capacity (the responsibility
they carry), and what was unified or split and why.

### The jobs table

Four columns, the main job first, then related and stakeholder jobs:

| Column | Holds |
|---|---|
| **Job** | The job's name (verb + object) in bold, linked to its entry if it has one; then, on a new line (`<br>`), its contextual clarifier where it has one. |
| **Category** | `Main`, `Sub-job` (a constituent the job map found separately mappable, once agreed worth mapping), `Related` (optionally with its place in time: `Related: before`, `after`, `alongside`) or `Stakeholder`. |
| **Executor** | The executor's name, as in the executors table. |
| **How it stands to the main job, and how its intent differs** | In words, how it touches the main job (for a higher-order job: *the main job is one means to it*) (*decides before the change is recorded*; *uses the roll to…*), its core intent, and the signal that makes it distinct (intent, time horizon, lifecycle, authority, language). Empty for the main job. Classifying relationships systematically is job domain analysis's work. |

Constituent candidates are not rows: they are listed on the main job's entry, and only there (a related job that is
mapped has none to take in). A constituent the job map finds separately
mappable, once agreed worth mapping, becomes a row, with category `Sub-job` and its own entry. A job is identified by its name; renames keep the old
name in its notes until citations are updated. A table cell cannot contain `|` or a line break other than `<br>`.

### The entries

`## Entries` holds a `###` section per job that has one, headed by its name, in table order. Directly under the
heading comes its YAML block when synced (see *Syncing*). Then a bullet list, written `**Name:**`, leaving out what
does not apply:

- **Statement**, **Category**, **Executor** and **Intent and difference**: as the row says. The statement stays
  concise ([jobs](jobs.md), *The core functional job*).
- **Scope**: what the job's object takes in and leaves out, with the edge cases that settled it.
- **Success criteria**: how the executor judges the whole job done well, in a phrase or two, with the standard for an
  assurance job. Not desired outcomes, which the job map writes.
- **Constituents** (the main job): a table of constituent candidates ([jobs](jobs.md), *Constituents of the main job*),
  as many as discovery turned up, not a complete decomposition:
  the candidate, what sets it off, what was noticed, the lean (*likely an episode*, *likely a step*, *possibly a job
  of its own*, *unclear*) and the status (*open* until a map has looked at it; then *covered:* with the steps; *separately
  mappable*, alone or with *covered*, with a link to its row and map once made; *outside scope:* with the job it
  belongs to; *unresolved:* with why).
- **Open classifications**: boundary questions the topology could not settle, with the evidence each way.
- **Map**: a link to its job map, if it has one; a link to the job domain analysis, if one covers it.
- **Edge cases**: the cases the object's breadth was tested against, and what they showed.
- **Qualifiers**: emotional and social, each labelled, only where evidence supports them.
- **Circumstances**: each, with what changes in it.
- **Seams**: where this job's execution leaves any system, and in which direction, if the framing does not already
  say.
- **Source**, and **Notes** (open questions start with *Open:*; candidates rejected as steps; stakeholder
  jobs considered and left out, with why, on the main job; executor questions).

### Drafts

A draft has the same shape, kept apart from the agreed topology (`job-topology.draft.md`, or the console). In a draft,
each job's name ends with its status, `[attested]`, `[inferred]` or `[proposed]`, and any other claim (an executor, a
category, a relation) whose status differs ends with its own mark. When the user agrees jobs into the topology they
move across without their marks; material doubt stays as an open question. Jobs proposed by a job map (its focus job
where it was made first, a higher-order job, a stakeholder job it found) are taken up the same way: proposed until
agreed here.

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
| **A diagram** | The main job in the centre with its constituents (and sub-jobs) inside it, related jobs beside it, stakeholder jobs outside with their executors and relations. Derived from the document, never drawn separately (Mermaid `flowchart` unless the project uses another). |
| **Part of a domain analysis** | Framing and topology first, ahead of the job maps. |

## Where it lives

In the folder that stands for the domain, beside its glossary (`job-topology.md`), with its job maps in a `job-maps/`
folder beside it, one per job. Ask if that is not evident. A synced topology is pushed and pulled as *Syncing* says.
