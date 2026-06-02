# PO Requirements Marketplace

A small [Claude Code](https://claude.com/claude-code) plugin marketplace containing the
**po-requirements** plugin — a guided interview skill that helps a product owner capture
clear, complete, *non-technical* project requirements and turn them into a structured
requirements document.

## What's inside

| Plugin | Skill | What it does |
|--------|-------|--------------|
| `po-requirements` | `po-requirements-gathering` | Runs a section-by-section requirements interview (problem, users, success, scope, process, risks) and produces a DRAFT requirements document for the product owner to confirm. |

## Install

In Claude Code, add this marketplace, then install the plugin:

```
/plugin marketplace add https://gitlab.com/<your-namespace>/po-requirements-marketplace.git
/plugin install po-requirements@po-requirements-marketplace
```

> Replace `<your-namespace>` with your GitLab username or group.

Once installed, the skill activates automatically when you ask to *gather requirements*,
*scope a project*, *write a brief*, or similar — or you can invoke it explicitly.

## Update

```
/plugin marketplace update po-requirements-marketplace
```

## Repository layout

```
.
├── .claude-plugin/
│   └── marketplace.json          # marketplace manifest (lists plugins)
├── plugins/
│   └── po-requirements/
│       ├── .claude-plugin/
│       │   └── plugin.json        # plugin manifest
│       └── skills/
│           └── po-requirements-gathering/
│               └── SKILL.md       # the skill itself
└── README.md
```

## License

MIT — see `LICENSE`.
