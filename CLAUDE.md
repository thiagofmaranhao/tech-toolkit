# CLAUDE.md — tech-toolkit · Thiago Maranhão

## Contexto do repositório

Repositório público de **Thiago Maranhão** (Software Architecture Manager) com artefatos técnicos extraídos de ambientes de produção real — templates, prompts e exemplos práticos nas áreas de **AI**, **sistemas distribuídos** e **arquitetura de software**.

Os artefatos são referência técnica antes de serem conteúdo: cada um foi validado em contexto real antes de ser publicado. Muitos estão vinculados a posts no LinkedIn e Medium, mas o repositório serve por conta própria como fonte de consulta e reutilização.

O repositório é aberto para uso e contribuição da comunidade.

## Estrutura

```
/
├── README.md                  # Apresentação do repositório e do autor
├── adr/                       # Templates e instruções para Architecture Decision Records
├── prompts/                   # Prompts reutilizáveis para ferramentas de AI (LLMs, Gems, etc.)
├── claude-code/               # Skills e hooks para Claude Code
├── dotnet/                    # Exemplos de código .NET/C# de produção
└── distributed-systems/       # Padrões e exemplos de sistemas distribuídos
```

> A estrutura cresce conforme novos artefatos são publicados. Cada pasta representa um domínio técnico, não um tipo de arquivo.

## Regras para novos artefatos

- Cada pasta agrupa artefatos por **contexto/domínio**, não por tipo de arquivo
- Todo artefato deve ser **originado ou validado em produção** — não é conteúdo teórico
- Toda pasta deve ter um `README.md` com:
  - O que é e para que serve
  - Contexto de produção onde foi usado (sem expor dados sensíveis)
  - Como usar
  - Seção **"Origem e referências"** com links dos posts que originaram ou mencionam os artefatos
- Artefatos devem ser autocontidos — quem chega pelo link do post deve conseguir usar sem contexto adicional
- Linguagem dos artefatos: **português** para documentação, inglês para código

## Ao criar uma nova pasta de artefatos

1. Criar a pasta com nome descritivo em kebab-case
2. Criar o `README.md` com estrutura padrão (contexto, como usar, referências)
3. Adicionar os artefatos
4. Atualizar o `README.md` raiz com a nova pasta

## Ao atualizar um artefato existente

- Manter compatibilidade com versões anteriores quando possível
- Se houver quebra, documentar o que mudou no `README.md` da pasta
- Atualizar a seção de referências se novos posts passarem a mencionar o artefato
