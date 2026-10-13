# Format and where it lives

## The analysis document

One Markdown document per domain, `job-domain-analysis.md`, beside the domain's `job-topology.md`. It **refers to the
topology's jobs by name** (linking to their entries) and never restates their definitions, so the two cannot disagree.
Any section may be absent; a partial analysis is normal.

````markdown
# Membership roll: job domain analysis

Analyses the jobs in the [job topology](job-topology.md). Open boundary questions taken up: whether providing
information about membership is one job or two; whether the relying parties are one executor.

## Identity between jobs

| Question | Conclusion | Evidence |
|---|---|---|
| Is providing information about membership one job or two? | One job | Routine and disputed requests share an objective (an information need met) and a completion; the disputed case is a circumstance |
| Are an insurer, a competition organiser and a venue one executor? | One (*relying party*) | Each needs to confirm someone belongs before relying on it: same objective, same completion |
| Is the treasurer's forecast part of the main job? | No: stakeholder | Different executor and intent (*what if*); uses the roll's numbers |

## Relationships

| Job | Executor | Relation | To | Notes |
|---|---|---|---|---|
| Decide on an application | Committee | governs | Maintain the membership roll | Bears on taking in a change |
| Join the club | Applicant | changes | Maintain the membership roll | |
| Resolve a membership dispute | Tribunal | governs | Maintain the membership roll | Bears on correcting the roll |

## Seams and obligations

- **Recording and effect:** under the club's rules membership may begin on entry in the roll (unverified); if so, the
  seam on taking in a change runs both ways.
- **Notices to the federation:** whether a notice completes a change or belongs to a separate reporting job is open.

## Boundary tests

- **A national federation at volume:** the same jobs; volume is a circumstance.
- **A club with no appointed secretary:** the same executor; the job is done by whoever holds the responsibility.

## Back to the topology

- Proposed: none; the topology's boundaries hold. (A rebuild of the roll is a constituent candidate for the job map,
  not a question for this analysis.)
````

### Sections

| Section | Holds |
|---|---|
| **Identity between jobs** | Each question taken up (one job or two; part of the main job or beside it; one executor or two), the conclusion and the evidence |
| **Relationships** | Each relationship: the job and its executor, the kind, the job it bears on, and, where it bears on only part of that job, which part |
| **Seams and obligations** | Each seam with its direction, and each obligation with where it is placed or why it is open |
| **Boundary tests** | The exceptional cases, settings and changes tried, and what they showed |
| **Back to the topology** | The changes to the topology the analysis proposes |

Evidence, drafts and syncing follow the topology's conventions (`job-topology` skill, *format*): status marks only in
drafts, open questions start with *Open:*, and IDs only when synced, in a YAML block under an entry's heading.

## Where it lives

Beside the domain's `job-topology.md` and glossary, in the folder that stands for the domain.
