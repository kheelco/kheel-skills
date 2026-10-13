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
| [job-topology](skills/job-topology/SKILL.md) | Surveys a domain's jobs: executors, the main functional job, and the adjacent and related jobs around it. Head of the job family ([README](skills/job-topology/README.md)). |
| [job-map](skills/job-map/SKILL.md) | Breaks one job into the steps its executor must accomplish, with the desired outcomes by which each step is judged. |

Each skill is a folder under `skills/` holding a `SKILL.md` and any `references/`, `assets/` or `scripts/` it needs.
