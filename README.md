# the-fakir-machine-skills-public

The public repository for all [Fakir IT](https://fakir-it.de) [Claude Code](https://claude.com/claude-code) skills and plugins.
This is where Fakir's reusable skills are stored, maintained, and distributed as a plugin marketplace.

## Available plugins & skills

| Plugin | Skill | What it does |
|--------|-------|--------------|
| `po-requirements` | `po-requirements-gathering` | Runs a section-by-section requirements interview (problem, users, success, scope, process, risks) and produces a DRAFT requirements document for the product owner to confirm. |

## Install

In Claude Code, add this marketplace, then install the plugin you need:

```
/plugin marketplace add https://github.com/fakir-tech/the-fakir-machine-skills-public.git
/plugin install po-requirements@the-fakir-machine-skills-public
```

Once installed, skills activate automatically on matching trigger phrases — or you can invoke them explicitly.

## Update

```
/plugin marketplace update the-fakir-machine-skills-public
```

## Repository layout

```
.
├── .claude-plugin/
│   └── marketplace.json          # marketplace manifest (lists all plugins)
├── plugins/
│   └── po-requirements/
│       ├── .claude-plugin/
│       │   └── plugin.json        # plugin manifest
│       └── skills/
│           └── po-requirements-gathering/
│               └── SKILL.md       # the skill itself
└── README.md
```

New plugins follow the same structure under `plugins/`.

## License

MIT — see `LICENSE`.
