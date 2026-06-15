# Cursor — Rules

Cursor rules extracted from real engineering workflows.

## Structure

```
cursor/
└── rules/
    └── <rule-name>.mdc    # Rule with YAML frontmatter + markdown instructions
```

Each rule follows the Cursor `.mdc` format and lives in `.cursor/rules/` in your project.

## Rules

| Rule | Description |
|------|-------------|
| [`generate-adr.mdc`](rules/generate-adr.mdc) | Generates an ADR from meeting notes or a refinement transcript |

## How to install a rule

Copy the `.mdc` file to your project's `.cursor/rules/` directory:

```bash
cp rules/generate-adr.mdc .cursor/rules/
```

Then invoke it by mentioning `@generate-adr` in a Cursor chat, or let the agent load it automatically based on context.

## Rule types used

| Type | Behavior |
|------|----------|
| Apply Intelligently (`alwaysApply: false`, description set) | Agent decides when to load based on the description |

## Origin and references

- Post: [Skills de IA para ADRs: como uso o Claude Code para padronizar documentação técnica](#) — coming soon
