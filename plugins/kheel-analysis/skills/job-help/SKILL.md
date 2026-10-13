---
name: job-help
description: >-
  Use when someone wants to understand Jobs to be Done as this plugin uses it, or wants to be guided through modelling
  the jobs in a domain: what a functional job, job executor, job map and desired outcome are; how the plugin follows
  Ulwick's Outcome-Driven Innovation and where it goes beyond it (job domain analysis, sub-jobs, episodes,
  circumstances and edge cases); which skill to use when; and what to do next. Trigger on "explain jobs to be done",
  "what is a job map", "what's a job executor", "what are desired outcomes", "how do I model the jobs in this domain",
  "where do I start", "walk me through it", "guide me through job modelling", "what's next", "is this Ulwick", "what's
  the difference between the topology and the map", "help with the job skills", or a newcomer's questions about any
  of the job skills.
---

# Job help

Explains the Jobs to be Done model used by the job skills, and guides people through modelling a domain's jobs. It
teaches and directs; it does not build artefacts. The artefacts are made by the other skills, which remain the
authority on how they are built:

| Skill | Makes |
|---|---|
| `glossary` | The domain's terms, which every job, step and outcome is written in |
| `job-topology` | The inventory of functional jobs and their executors |
| `job-domain-analysis` | Optional: how the jobs fit together |
| `job-map` | A job's steps over the eight universal stages, with desired outcomes |

## Two modes

**Explaining.** Answer the question asked, at the depth asked, in plain language, with an example from the person's
own domain where one is to hand, otherwise from a neutral one (a club's membership roll, a fleet of vehicles). Say
plainly what comes from Ulwick and what is this plugin's own extension ([extensions](references/extensions.md)). Do
not lecture: one concept, its example, and an offer to go further.

**Guiding.** Take the person through modelling their domain, one stage at a time ([guide](references/guide.md)):

1. find out where they are (nothing yet; notes or interviews to hand; a glossary; a topology; maps);
2. say what the next stage is, what it produces, why it comes now, and roughly how much it involves;
3. ask the one or two questions that start it, or hand over to the skill that does it;
4. when a stage is done, check it against the stage's *ready to move on* test, then offer the next.

Let the person skip or reorder stages; the guide is a recommendation, not a gate. Never invent the domain's content
to keep the process moving: an unanswered question is recorded as open, and the guide moves on or waits.

## Principles

- **Plain first.** Lead with what something is for and an example; bring in the formal terms (*functional job*,
  *desired outcome*) once the idea has landed.
- **Honest about provenance.** Ulwick's Outcome-Driven Innovation provides the core: functional jobs, executors,
  related and emotional jobs, the eight-stage job map, desired outcome statements and opportunity scoring. The job
  topology artefact, open classifications, job domain analysis, sub-jobs, episodes, variants for circumstances and edge
  cases, and seams are this plugin's own, consistent with Ulwick but not part of his method. Never present them as
  canonical Ulwick.
- **Point, do not duplicate.** Summarise a rule to explain it; for the rule itself, name the skill and reference
  that holds it.
- **Their domain, not a product.** Jobs describe what people are trying to get done whether or not any system exists.
  Steer gently away from screens, features and workflows when they creep in.

## Reference

| File | Holds |
|---|---|
| [references/concepts.md](references/concepts.md) | The JTBD concepts, each with a plain explanation and an example |
| [references/extensions.md](references/extensions.md) | What is Ulwick and what is this plugin's extension, and when the extension is worth using |
| [references/guide.md](references/guide.md) | The modelling process, stage by stage, with the questions that start each and the test for moving on |
| [references/faq.md](references/faq.md) | Common questions and confusions |

For questions about the underlying model (the generic activity model, the family's profiles, mapping to other
systems), draw on [README.md](README.md), the job family's reference.
