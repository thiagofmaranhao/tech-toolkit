# ADR — Architecture Decision Records

## What it is

A collection of artifacts for generating Architecture Decision Records (ADRs) with AI assistance. The workflow cuts ADR creation from hours to minutes by combining a Gemini Pro Gem with a standardized template and prompt.

## Artifacts

| File | Description |
|------|-------------|
| [`gem-instructions.md`](gem-instructions.md) | Instructions that configure the Gemini Pro Gem as an ADR generator |
| [`template-adr.md`](template-adr.md) | ADR template consumed by the Gem to produce structured decisions |
| [`prompt-generate-adr.md`](prompt-generate-adr.md) | Standard prompt to trigger ADR generation right after a meeting or decision session |

## How to use

1. Create a Gemini Pro Gem using the instructions in [`gem-instructions.md`](gem-instructions.md)
2. Upload or paste [`template-adr.md`](template-adr.md) as the Gem's reference template
3. After a meeting or decision session, use the prompt in [`prompt-generate-adr.md`](prompt-generate-adr.md) to generate a draft ADR
4. Review, adjust, and commit the ADR to your repository

## Origin and references

- Post: [De 4 horas para 10 minutos: como passei a criar ADRs com IA logo após a reunião](https://www.linkedin.com/posts/activity-7468730068161273856-VqqS?utm_source=share&utm_medium=member_desktop&rcm=ACoAAAGcx-4B68luVeo0Z18FVACS6U_EoiW3o4M) — Jun 5, 2026
