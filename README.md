# kheel-skills

A Claude Code plugin marketplace holding Kheel's skill plugins.

## Plugins

| Plugin | What it does |
|---|---|
| [kheel-analysis](plugins/kheel-analysis/README.md) | Requirements analysis: glossary (ontology), activity mapping, domain modelling, use cases, stories, business rules and constraints. |

## Installing

```
/plugin marketplace add kheelco/kheel-skills
/plugin install kheel-analysis@kheel-skills
```

From a local clone, add the marketplace by its path instead: `/plugin marketplace add ./kheel-skills`.

## Repository layout

```
kheel-skills/
├── .claude-plugin/
│   └── marketplace.json        # lists the plugins; makes this repo installable as a marketplace
└── plugins/
    └── kheel-analysis/
        ├── .claude-plugin/
        │   └── plugin.json
        ├── README.md
        └── skills/             # one folder per skill, each with a SKILL.md
```

## Adding a plugin

Create `plugins/<name>/` with a `.claude-plugin/plugin.json`, a `README.md` and a `skills/` folder, then add an
entry for it to `.claude-plugin/marketplace.json` and the table above.
