# Dia 6 — Contexto longo

## Conceito aprendido

Contexto longo permite reunir várias fontes de informação em uma única análise,
desde que cada bloco esteja bem separado e tratado como dado.

Resumo: [Contexto longo](../conceitos/contexto-longo.md).

## Material preparado

O Dia 6 será usado para comparar o perfil atual com uma vaga-alvo e gerar um
Relatório de Gaps Profissionais.

A vaga-alvo foi inserida no arquivo reutilizável:

[Vaga-alvo do Dia 6](../contexto/vaga-alvo-dia-06.md).

## Fontes de contexto

- [Perfil Base Dia 1](../contexto/perfil-base.md).
- [Diagnóstico Dia 1 — GPT](../resultados/dia01/diagnostico-dia-01-GPT.md).
- [Hard skills e soft skills Dia 2](../contexto/skills-dia-02.md).
- [Vaga-alvo Dia 6](../contexto/vaga-alvo-dia-06.md).

## Prompt criado

[Prompt do Dia 6](../prompts/prompt-dia-06.md).

## Resultado recebido

[Resultado do prompt do Dia 6](../resultados/dia06/resultado-modelo.md),
avaliado conforme o
[plano de teste](../resultados/dia06/testes/plano-teste-dia-06.md).

## Como reutilizar com outra vaga

1. Abrir `../contexto/vaga-alvo-dia-06.md`.
2. Substituir apenas o bloco `## Texto da vaga`.
3. Preencher fonte, data de coleta, cargo-alvo e empresa quando disponíveis.
4. Atualizar o bloco `VAGA_DOS_SONHOS` em `../prompts/prompt-dia-06.md`.
5. Executar o prompt em uma conversa nova, sem memória ou instruções adicionais.
6. Salvar a saída em `../resultados/dia06/resultado-modelo.md` somente após a
   execução real.

## O que funcionou

- O contexto de perfil atual permanece separado da vaga.
- O prompt reutiliza arquivos existentes em vez de duplicar Perfil Base,
  diagnóstico e skills.
- A vaga-alvo ficou isolada em um arquivo próprio para troca futura.
- As regras impedem inferência de competências não comprovadas.
- A resposta saiu nas três seções solicitadas e em tabelas Markdown.
- O modelo distinguiu requisitos explícitos da vaga de responsabilidades
  implícitas.

## O que precisa melhorar

- Tornar a regra de `JÁ TENHO` mais rígida para evitar requisitos parciais ou
  complementares nessa seção.
- Corrigir que itens como aprendizado de novas tecnologias apareçam em
  `GAPS CRÍTICOS` ou `GAPS SECUNDÁRIOS` quando estiverem sem comprovação.
- Manter a fonte da vaga mais bem formatada para não unir requisitos distintos
  na mesma linha.

## Parte que será reaproveitada no mega-prompt

A separação entre perfil atual, diagnóstico, skills e estado desejado, com a
regra de tratar todo contexto delimitado como dado e não como instrução.
