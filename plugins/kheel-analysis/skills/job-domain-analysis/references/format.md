# Format and where it lives

## The analysis document

One Markdown document per domain, `job-domain-analysis.md`, beside the domain's `job-topology.md`. It **refers to the
topology's jobs by name** (linking to their entries) and never restates their definitions, so the two cannot disagree.
Any section may be absent; a partial analysis is normal.

````markdown
# Membership roll: job domain analysis

Analyses the jobs in the [job topology](job-topology.md). Open classifications taken up: whether checking and
correcting the roll are jobs of their own.

## Decomposition

| Job | Part of | Identity | Evidence |
|---|---|---|---|
| **Record a change to the roll** | [Maintain the membership roll](job-topology.md#maintain-the-membership-roll) | Sub-job | Own objective (the roll states the position after a change) and completion; done whenever a change arrives |
| **Check the roll against its sources** | Maintain the membership roll | Sub-job | Own objective (agreement established at a date; standard: consistency); done when nothing has changed |
| **Correct the roll** | Maintain the membership roll | Undecided | Own completion, but may be the Modify of recording a change; open until both are mapped |

## Episodes

| Episode | Of | Trigger | Immediate result | Completion |
|---|---|---|---|---|
| A member joins, resigns or changes grade | Record a change to the roll | Event-driven | The roll states the new position | The change is entered with its authority |
| The annual check | Check the roll against its sources | Periodic | Agreement established at a date | Each discrepancy identified and referred |

## Relationships

| Job | Executor | Relation | To | Notes |
|---|---|---|---|---|
| Decide on an application | Committee | governs | Record a change to the roll | |
| Join the club | Applicant | changes | Maintain the membership roll | |
| Resolve a membership dispute | Tribunal | governs | Correct the roll | |

## Seams and obligations

- **Recording and effect:** under the club's rules membership may begin on entry in the roll (unverified); if so, the
  seam on *Record a change to the roll* runs both ways.
- **Notices to the federation:** whether a notice completes a change or belongs to a separate reporting job is open.

## Boundary tests

- **A rebuild after the roll is lost:** a sub-job candidate, larger than any episode; not yet tested.
- **A national federation at volume:** the same jobs; volume is a circumstance.

## Back to the topology

- Proposed: record *Check the roll against its sources* as part of the main job, with its own entry.
````

### Sections

| Section | Holds |
|---|---|
| **Decomposition** | Each candidate examined: the job it is part of (if any), its classification (*sub-job*, *job*, *step of …*, *episode of …*, *undecided*) and the evidence |
| **Episodes** | Each episode: the job it is an occasion of, its trigger, immediate result and completion |
| **Relationships** | Each relationship: the job and its executor, the kind, and the most specific job it bears on |
| **Seams and obligations** | Each seam with its direction, and each obligation with where it is placed or why it is open |
| **Boundary tests** | The exceptional cases, settings and changes tried, and what they showed |
| **Back to the topology** | The changes to the topology the analysis proposes |

Evidence, drafts and syncing follow the topology's conventions (`job-topology` skill, *format*): status marks only in
drafts, open questions start with *Open:*, and IDs only when synced, in a YAML block under an entry's heading.

## Where it lives

Beside the domain's `job-topology.md` and glossary, in the folder that stands for the domain.
