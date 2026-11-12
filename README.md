# kheel-skills

A Claude Code plugin marketplace holding Kheel's skill plugins.

Copyright © 2026 Jeremy Buckley. Source-available under the [PolyForm Shield License 1.0.0](LICENSE.md): free
to use, including commercially, but not to build into a product that competes with it or with Kheel. See
[Licence](#licence).

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
├── LICENSE.md                  # PolyForm Shield 1.0.0; copied into each skill folder
└── plugins/
    └── kheel-analysis/
        ├── .claude-plugin/
        │   └── plugin.json
        ├── README.md
        └── skills/             # one folder per skill, each with a SKILL.md and a copy of LICENSE.md
```

## Adding a plugin

Create `plugins/<name>/` with a `.claude-plugin/plugin.json` (with `"license": "PolyForm-Shield-1.0.0"`), a
`README.md` and a `skills/` folder, then add an entry for it to `.claude-plugin/marketplace.json` and the table
above. Every skill folder carries `LICENSE.md`, an exact copy of the one at the repository root, so the licence
travels with a skill however it is installed; copy it into each new skill.

## Licence

Copyright © 2026 Jeremy Buckley. All rights not granted by the licence are reserved.

This repository — the plugins, their skills and everything they carry — is source-available under the
**[PolyForm Shield License 1.0.0](LICENSE.md)**. It is not open source, and it does not convert to an open-source
licence later.

In short (the [licence text](LICENSE.md) is what governs):

- **You may** use it for any purpose that doesn't compete — analysing domains and requirements for your own
  products, internal use, work you do for clients, education and research — and change it and share it for those
  purposes. What you produce with the skills is yours.
- **You may not** use it to provide a product or service that competes with it, or with any product the
  licensor or its affiliates provides using it, such as Kheel. That includes bringing the skills, changed or not,
  into another product. A product competes even if it is free, runs on a different platform or is written in a
  different language.
- **Permission** for anything outside those terms, including use in another product, is by separate written
  agreement with the licensor — email [info@kheel.co](mailto:info@kheel.co) to ask.

If you pass on any part of it, include the licence (or its URL) and the `Required Notice:` line at the top of
[LICENSE.md](LICENSE.md). Each skill folder carries its own copy of `LICENSE.md`, so the terms travel with a
skill however it is installed.
