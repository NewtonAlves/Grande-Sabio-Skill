# Memória Local

Projeto longo precisa de memória. Sem registro, decisões se perdem, personagens mudam sem intenção, o mundo contradiz a si mesmo e a revisão volta sempre aos mesmos problemas.

A **Grande Sabio** usa uma pasta chamada `project-memory/` para guardar o estado real da obra.

Essa pasta deve ficar no projeto da obra, não dentro da pasta da skill.

## Estrutura Recomendada

```text
project-memory/
├── PROJECT_STATE.md
├── PROGRESS_LOG.md
├── TODO.md
├── PENDING_DECISIONS.md
├── DECISIONS.md
├── STYLE_GUIDE.md
├── AUTHOR_VOICE.md
├── CHARACTERS.md
├── WORLD_BIBLE.md
├── TIMELINE.md
├── LOCATIONS.md
├── GLOSSARY.md
├── NAMES_BANK.md
├── CONTINUITY_LOG.md
├── REVISION_NOTES.md
├── SOURCES.md
└── SESSION_SUMMARIES.md
```

Os modelos ficam em `templates/`.

## Função Dos Arquivos

| Arquivo | Função |
| --- | --- |
| `PROJECT_STATE.md` | estado geral da obra |
| `PROGRESS_LOG.md` | registro do que foi feito |
| `TODO.md` | tarefas abertas |
| `PENDING_DECISIONS.md` | decisões ainda não tomadas |
| `DECISIONS.md` | decisões confirmadas |
| `STYLE_GUIDE.md` | tom, linguagem e padrão editorial |
| `AUTHOR_VOICE.md` | voz autoral e escolhas que devem ser preservadas |
| `CHARACTERS.md` | personagens, arcos, relações e estado atual |
| `WORLD_BIBLE.md` | mundo ficcional, regras, culturas e sistemas |
| `TIMELINE.md` | linha do tempo da obra |
| `LOCATIONS.md` | locais importantes |
| `GLOSSARY.md` | termos aprovados e termos a evitar |
| `NAMES_BANK.md` | nomes aprovados, em teste e rejeitados |
| `CONTINUITY_LOG.md` | contradições, correções e pontos a conferir |
| `REVISION_NOTES.md` | notas de revisão e problemas recorrentes |
| `SOURCES.md` | fontes externas consultadas |
| `SESSION_SUMMARIES.md` | resumo de cada sessão |

## Fluxo Recomendado

1. Criar `project-memory/` no projeto da obra.
2. Copiar os templates necessários.
3. Preencher `PROJECT_STATE.md`.
4. Registrar voz e estilo em `STYLE_GUIDE.md` e `AUTHOR_VOICE.md`.
5. Registrar personagens, mundo, linha do tempo e nomes.
6. Escrever, revisar, diagnosticar ou continuar a obra.
7. Atualizar decisões, pendências e progresso ao final da sessão.

## Atualização Manual

Quando não houver permissão de escrita, a skill deve entregar um bloco pronto para atualização manual.

```markdown
## Atualização manual da memória

Arquivo: project-memory/DECISIONS.md

Conteúdo sugerido:
- Decisão:
- Motivo:
- Impacto na obra:
```

## Fontes Consultadas

Quando uma fonte externa for usada para decidir uma regra de português brasileiro, fato real ou padrão editorial, ela deve ser registrada em `SOURCES.md`.

```markdown
### AAAA-MM-DD - Tema consultado

- Fonte:
- Link:
- Motivo da consulta:
- Conclusão:
- Aplicação na obra:
```

## Regra Principal

Memória local não é enfeite. Ela serve para manter continuidade, reduzir retrabalho e proteger a obra de decisões contraditórias.

