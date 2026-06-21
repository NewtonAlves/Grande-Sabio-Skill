# Exemplo: Diálogo Ramificado De Jogo

## Pedido Do Usuário

Use $grande-sabio para criar um diálogo ramificado para um RPG brasileiro de fantasia sombria. O jogador encontra uma barqueira que sabe onde fica a cidade submersa, mas ela não confia em forasteiros.

## Contexto

- Formato: diálogo interativo.
- Função de gameplay: liberar rota, criar custo narrativo e registrar consequência.
- Tom: sombrio, direto e com subtexto.
- Limite: escolhas precisam alterar informação, relação ou risco.

## Modo Aplicado

- Narrativa Para Jogos.
- Criador De Personagens.
- Criador De Mundo.

## Entrega Da Skill

### NPC

Nome: Dália Da Várzea.

Função: barqueira que conhece a rota para a cidade submersa.

Voz: fala pouco, usa imagens de rio e evita responder perguntas diretas.

Medo: levar outro forasteiro até a cidade e vê-lo voltar diferente.

### Entrada Da Cena

Dália prende a corda do barco no tronco encharcado e olha para as botas limpas do jogador.

> "Quem pisa seco demais costuma afundar primeiro."

### Escolhas Do Jogador

1. "Eu pago pela travessia."
   - Resposta: "Moeda afunda igual pedra."
   - Consequência: Dália recusa dinheiro, mas revela que aceita outro tipo de garantia.
   - Estado: `dalia_confia = false`, `rota_revelada = false`.

2. "Estou procurando alguém que entrou na cidade."
   - Resposta: "Nome?"
   - Consequência: se o jogador disser um nome registrado em missão anterior, Dália reconhece e oferece travessia parcial.
   - Estado: `dalia_confia = parcial`, `rota_revelada = parcial`.

3. "Você tem medo daquele lugar."
   - Resposta: "Tenho memória. Medo é coisa de quem ainda acha que pode escolher."
   - Consequência: aumenta tensão, mas abre pergunta sobre o passado dela.
   - Estado: `dalia_passado_desbloqueado = true`.

4. "Não vou obrigar você. Só me diga o que devo evitar."
   - Resposta: "Não responda quando a água chamar pelo seu nome."
   - Consequência: Dália entrega uma regra de sobrevivência e permite nova abordagem depois.
   - Estado: `regra_agua_nome = true`, `dalia_confia = parcial`.

### Consequência Narrativa Recomendada

Se o jogador insistir em dinheiro ou ameaça, Dália não revela a rota completa. Se demonstrar respeito pelo medo dela ou trouxer um nome relevante, a travessia começa, mas o jogador recebe uma regra de risco: nunca responder à água quando ela chamar.

## Atualização De Memória Local

Arquivo: `project-memory/CHARACTERS.md`

```markdown
### Dália Da Várzea

- Papel narrativo: barqueira e guardiã informal da rota para a cidade submersa.
- Desejo externo: impedir que forasteiros despreparados entrem na cidade.
- Medo interno: repetir uma travessia que terminou em perda.
- Voz: frases curtas, imagens de rio, respostas indiretas.
```

Arquivo: `project-memory/WORLD_BIBLE.md`

```markdown
## Cidade submersa

- Regra: a água pode chamar pessoas pelo nome.
- Consequência: responder ao chamado cria risco narrativo ainda a definir.
- Relação: Dália conhece a rota, mas só guia quem respeita seus limites.
```

Arquivo: `project-memory/CONTINUITY_LOG.md`

```markdown
### AAAA-MM-DD - Regra da água que chama pelo nome

- Problema: definir o que acontece se o jogador responder.
- Impacto: afeta missão, lore e possíveis finais.
- Status: pendente.
```

## Observação Técnica

Este exemplo demonstra narrativa interativa com escolhas que mudam relação, informação e risco. Ele evita diálogo decorativo e mostra como registrar consequência de jogo na memória local.

