# Claude Code — Skills

Skills for Claude Code extracted from real engineering workflows.

## Structure

```
claude-code/
└── skills/
    └── <skill-name>/
        ├── SKILL.md          # Main skill instructions and frontmatter
        └── [supporting files]
```

Each skill follows the [Agent Skills](https://agentskills.io) open standard and can be installed at the personal (`~/.claude/skills/`) or project (`.claude/skills/`) level.

## Skills

| Skill | Command | Description |
|-------|---------|-------------|
| [`generate-adr`](skills/generate-adr/) | `/generate-adr` | Generates an ADR from meeting notes or a refinement transcript |

## How to install a skill

**Personal (available in all your projects):**
```bash
cp -r skills/generate-adr ~/.claude/skills/
```

**Project-level (available in the current project only):**
```bash
cp -r skills/generate-adr .claude/skills/
```

Then invoke it with `/generate-adr [brief decision summary]` or let Claude load it automatically when relevant.

## Origin and references

- Post: [Skills de IA para ADRs: como uso o Claude Code para padronizar documentação técnica](#) — coming soon
