# kheel-analysis

Agent skills for requirements analysis at various levels of detail, from the language of a domain down to the
rules a system must enforce:

- **Glossary (ontology):** the terms the domain uses, what they mean and how they relate.
- **Activity modelling:** what people in the domain are trying to get done (Jobs to be Done), what it takes, and how
  they judge it done well.
- **Domain modelling:** the concepts, their relationships and their lifecycles.
- **Use cases and stories:** what actors achieve with the system.
- **Business rules and constraints:** what must always hold, and the limits the solution works within.

## Skills

| Skill | What it does |
|---|---|
| [glossary](skills/glossary/SKILL.md) | Develops and maintains the glossary (language model, conceptual model, vocabulary): terms, their boundaries and relations, rules and variation, reviews, diagrams and syncing. |
| [job-topology](skills/job-topology/SKILL.md) | Ulwick-aligned discovery of a domain's functional jobs: executors, the main job, the adjacent and related jobs around it, and what is left open. Head of the job family. |
| [job-domain-analysis](skills/job-domain-analysis/SKILL.md) | Optional extension: how the jobs fit together (identity, sub-jobs, episodes, relationships, seams, obligations, boundary tests). |
| [job-map](skills/job-map/SKILL.md) | Breaks one job into the steps its executor must accomplish, with the desired outcomes by which each step is judged. |
| [job-help](skills/job-help/SKILL.md) | Explains the Jobs to be Done model, what is Ulwick and what is the extension, and guides people through modelling a domain's jobs stage by stage. Its [README](skills/job-help/README.md) describes the job family and its generic activity model. |

Each skill is a folder under `skills/` holding a `SKILL.md` and any `references/`, `assets/` or `scripts/` it needs.
