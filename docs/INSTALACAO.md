# Instalação

Guia de instalação da skill `grande-sabio`.

## Dados Do Repositório

| Item | Valor |
| --- | --- |
| Criador | Newton Alves |
| GitHub | [NewtonAlves](https://github.com/NewtonAlves) |
| Nome visível | `Grande Sabio` |
| Nome técnico | `grande-sabio` |
| Repositório sugerido | `Grande-Sabio-Skill` |
| Idioma | Português brasileiro |

## Instalar Pelo GitHub

Com o repositório publicado, use:

```bash
npx skills add NewtonAlves/Grande-Sabio-Skill
```

Se o repositório tiver outro slug, ajuste o comando:

```bash
npx skills add NewtonAlves/<nome-do-repositorio>
```

## Conferir Se A Skill Foi Encontrada

Depois da instalação, chame a skill em uma conversa:

```text
Use $grande-sabio para revisar este trecho em português brasileiro mantendo minha voz.
```

Se a instalação estiver correta, o agente deve reconhecer a skill `grande-sabio` e aplicar suas regras editoriais.

## Regras Que Não Devem Mudar

- O nome técnico deve permanecer `grande-sabio`.
- O nome visível aprovado é `Grande Sabio`.
- O idioma padrão é português brasileiro.
- O foco é escrita editorial, literária e narrativa.
- A skill não deve usar português europeu como padrão.
- A memória real de uma obra deve ficar no projeto da obra, não dentro da pasta da skill.

## Estrutura Esperada

```text
grande-sabio/
├── SKILL.md
├── README.md
├── agents/
├── docs/
├── examples/
├── references/
└── templates/
```

O arquivo obrigatório para funcionamento da skill é `SKILL.md`. Os demais arquivos organizam interface, documentação, exemplos, referências e templates.

