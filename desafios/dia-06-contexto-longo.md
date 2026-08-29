# Dia 6 — Contexto longo

## Conceito aprendido

Contexto longo permite reunir várias fontes de informação em uma única análise,
desde que cada bloco esteja bem separado e tratado como dado.

Resumo: [Contexto longo](../conceitos/contexto-longo.md).

## Material preparado

O Dia 6 será usado para comparar o perfil atual com uma vaga-alvo e gerar um
Relatório de Gaps Profissionais.

A vaga-alvo foi inserida no arquivo reutilizável:

[Vaga-alvo BairesDev Python Jr](../contexto/vagas/bairesdev-python-jr-2026-08-27.md).

## Fontes de contexto

- [Perfil Base Dia 1](../contexto/perfil-base.md).
- [Diagnóstico Dia 1 — GPT](../resultados/dia01/diagnostico-dia-01-GPT.md).
- [Hard skills e soft skills Dia 2 — GPT](../contexto/derivados/skills-dia-02-gpt.md).
- [Vaga-alvo BairesDev Python Jr](../contexto/vagas/bairesdev-python-jr-2026-08-27.md).

## Prompt criado

[Template do prompt do Dia 6](../prompts/prompt-dia-06.md).

O prompt final executado foi preservado como snapshot em
[prompt-final-2026-08-27-gpt-5-5.md](../resultados/dia06/prompt-final-2026-08-27-gpt-5-5.md).

As fontes usadas nessa execução estão registradas no
[manifesto de contexto](../resultados/dia06/contexto-manifest.md).

## Resultado recebido

[Resultado da primeira execução do Dia 6](../resultados/dia06/resultado-modelo.md),
avaliado com ressalvas conforme o
[plano de teste](../resultados/dia06/testes/plano-teste-dia-06.md).

Após a revisão, o prompt recebeu ajustes mínimos e foi registrada uma
[execução complementar](../resultados/dia06/resultado-complementar-ajustes-dia-06.md).

## Como reutilizar com outra vaga

1. Criar uma nova vaga em `../contexto/vagas/`.
2. Preencher fonte, data de coleta, cargo-alvo, empresa e texto integral da vaga.
3. Copiar `../prompts/prompt-dia-06.md` para um arquivo de prompt final da nova
   execução.
4. Substituir os placeholders do prompt final pelos conteúdos integrais das
   fontes escolhidas.
5. Registrar as fontes em um manifesto de contexto da execução.
6. Executar o prompt final em uma conversa nova, sem memória ou instruções
   adicionais.
7. Salvar a saída em `../resultados/dia06/resultado-modelo.md` somente após a
   execução real.

## O que funcionou

- O contexto de perfil atual permanece separado da vaga.
- O prompt final preserva um snapshot dos dados usados na execução.
- O template do prompt pode ser reutilizado sem editar o snapshot anterior.
- A vaga-alvo ficou isolada em um arquivo próprio para troca futura.
- As regras impedem inferência de competências não comprovadas.
- A resposta saiu nas três seções solicitadas e em tabelas Markdown.
- O modelo distinguiu requisitos explícitos da vaga de responsabilidades
  implícitas.
- A execução complementar manteve `JÁ TENHO` restrito a requisitos comprovados
  e moveu itens parciais ou ambíguos para gaps.

## O que precisa melhorar

- Preservar a distinção entre a primeira execução com ressalvas e a execução
  complementar consolidada.
- Manter a regra de `JÁ TENHO` rígida para evitar requisitos parciais,
  complementares ou que requeiram confirmação nessa seção em novas execuções.
- Manter a fonte da vaga mais bem formatada para não unir requisitos distintos
  na mesma linha.

## Parte que será reaproveitada no mega-prompt

A separação entre perfil atual, diagnóstico, skills e estado desejado, com a
regra de tratar todo contexto delimitado como dado e não como instrução.
