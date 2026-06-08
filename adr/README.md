# ADR — Architecture Decision Records

## What it is

A collection of artifacts for generating Architecture Decision Records (ADRs) with AI assistance. The workflow cuts ADR creation from hours to minutes by combining a Gemini Pro Gem with a standardized template and prompt.

## Artifacts

| File | Description |
|------|-------------|
| [`template-adr.md`](template-adr.md) | ADR template used by all AI assistants to produce structured decisions |
| [`gem-instructions.md`](gem-instructions.md) | Instructions to configure a Gemini Pro Gem as an ADR generator |
| [`claude-instructions.md`](claude-instructions.md) | Instructions to configure a Claude Project as an ADR generator |
| [`chatgpt-instructions.md`](chatgpt-instructions.md) | Instructions to configure a ChatGPT Custom GPT as an ADR generator |
| [`prompt-generate-adr.md`](prompt-generate-adr.md) | Standard prompt to trigger ADR generation right after a meeting or decision session |

## How to use

1. Pick your AI tool and follow the corresponding instructions file to set up the assistant
2. Upload [`template-adr.md`](template-adr.md) to the assistant's knowledge base
3. After a meeting or decision session, use the prompt in [`prompt-generate-adr.md`](prompt-generate-adr.md) to generate a draft ADR
4. Review, adjust, and commit the ADR to your repository

## Origin and references

- Post: [De 4 horas para 10 minutos: como passei a criar ADRs com IA logo após a reunião](https://www.linkedin.com/posts/activity-7468730068161273856-VqqS?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAGcx-4B68luVeo0Z18FVACS6U_EoiW3o4M) — Jun 5, 2026
- Post: [tech-toolkit — repositório público com artefatos de engenharia extraídos de produção](https://www.linkedin.com/posts/activity-7469893522784169984-yqn1?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAGcx-4B68luVeo0Z18FVACS6U_EoiW3o4M) — Jun 8, 2026
