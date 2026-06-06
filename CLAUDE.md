# CLAUDE.md — tech-toolkit · Thiago Maranhão

## Language

All content in this repository — documentation, README files, artifact descriptions, and AI-generated output — must be written in **English**. Code was always in English; now documentation follows the same rule.

## Repository context

Public repository by **Thiago Maranhão** (Software Architecture Manager) with engineering artifacts extracted from real production environments — templates, prompts, and practical examples across **AI**, **distributed systems**, and **software architecture**.

Artifacts are technical references first, content second: each one was validated in a real context before being published. Many are linked to posts on LinkedIn and Medium, but the repository stands on its own as a reference and reuse source.

Open for community use and contribution.

## Structure

```
/
├── README.md                  # Repository and author overview
├── adr/                       # Templates and instructions for Architecture Decision Records
├── prompts/                   # Reusable prompts for AI tools (LLMs, Gems, etc.)
├── claude-code/               # Skills and hooks for Claude Code
├── dotnet/                    # Production .NET/C# code examples
└── distributed-systems/       # Distributed systems patterns and examples
```

> The structure grows as new artifacts are published. Each folder represents a technical domain, not a file type.

## Rules for new artifacts

- Each folder groups artifacts by **domain/context**, not by file type
- Every artifact must be **originated or validated in production** — no purely theoretical content
- Every folder must have a `README.md` with:
  - What it is and what it's for
  - Production context where it was used (without exposing sensitive data)
  - How to use it
  - **"Origin and references"** section with links to posts that originated or mention the artifacts
- Artifacts must be self-contained — someone arriving from a post link should be able to use them without additional context

## Adding a new artifact folder

1. Create the folder with a descriptive kebab-case name
2. Create the `README.md` with the standard structure (context, how to use, references)
3. Add the artifacts
4. Update the root `README.md` with the new folder

## Updating an existing artifact

- Maintain backward compatibility when possible
- If there's a breaking change, document what changed in the folder's `README.md`
- Update the references section if new posts start mentioning the artifact

## Commit convention

Follow [Conventional Commits](https://www.conventionalcommits.org/). Format: `<type>(<scope>): <description>`

**Scope is mandatory** and must be the artifact folder name (e.g. `adr`, `prompts`, `dotnet`). For changes affecting the repository as a whole, use `repo`.

**Types:**
| Type | When to use |
|------|-------------|
| `feat` | New artifact or new functionality in an existing artifact |
| `fix` | Correction in an existing artifact |
| `docs` | Change in README or documentation |
| `refactor` | Reorganization without content or behavior change |
| `chore` | General maintenance (`.gitignore`, configs, renames) |

**Examples:**
```
feat(adr): add ADR template for distributed systems decisions
docs(prompts): update README with Claude Code usage examples
fix(dotnet): correct dependency injection example
chore(repo): add .gitignore
```
