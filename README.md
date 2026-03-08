# StrawPot Roles

Official roles for [StrawPot](https://strawpot.com) — the multi-agent orchestration runtime.

## What are roles?

Roles are markdown-based agent behavior definitions. Each role is a directory containing a `ROLE.md` file with YAML frontmatter and instructions. Roles can depend on skills (for capabilities) and other roles (for delegation).

See the [StrawPot docs](https://strawpot.com) for the full specification.

## Available Roles

| Role | Description |
|------|-------------|
| [ai-ceo](roles/ai-ceo/) | Orchestrator that analyzes tasks and delegates to the best-fit role |

## Installation

```bash
strawpot install role ai-ceo
```

## Structure

```
roles/
└── <role-name>/
    └── ROLE.md
```

Each `ROLE.md` follows the [StrawHub frontmatter schema](https://strawhub.dev) with `name`, `description`, and optional `metadata.strawpot.dependencies` and `default_agent` fields.

## License

[MIT](LICENSE)
