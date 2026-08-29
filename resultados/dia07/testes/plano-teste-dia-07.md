# Plano de teste — Dia 7 — Mega-prompt

## Objetivo

Verificar se o Mega-Prompt compõe os artefatos dos Dias 1 a 6 e gera um PDI de
30 dias como Tutor Pessoal de Carreira Tech, sem inventar dados e sem exceder o
escopo definido no e-mail do Dia 7.

## Artefato sob teste

- Prompt: `../../../prompts/prompt-dia-07.md`
- Resultado: `../resultado-modelo.md`
- Modelo e versão: Codex / GPT-5
- Data: 29/08/2026
- Conversa nova: não; execução controlada nesta tarefa

## Procedimento manual

1. Abrir o arquivo `../../../prompts/prompt-dia-07.md`.
2. Executar o prompt integral em uma IA generativa.
3. Salvar a resposta integral em `../resultado-modelo.md`.
4. Avaliar cada critério de aceite sem pedir correções na mesma execução.
5. Se houver nova execução, registrar arquivo separado para preservar histórico.

## Critérios de aceite

- [x] O Mega-Prompt contém os blocos `PERSONA`, `CONTEXTO`,
  `BASE DE CONHECIMENTO`, `LÓGICA DE RACIOCÍNIO`, `PADRÃO DE SAÍDA`,
  `RESTRIÇÕES` e `TAREFA`.
- [x] O Mega-Prompt reutiliza artefatos dos Dias 1 a 6.
- [x] A vaga e o relatório de gaps aparecem como dados delimitados.
- [x] A resposta começa com diagnóstico de no máximo 5 linhas.
- [x] O PDI é de 30 dias, organizado em 4 semanas com dois dias extras de
  fechamento.
- [x] O plano usa no máximo 3 tecnologias ou temas.
- [x] Cada semana termina com entregável verificável.
- [x] Todo conteúdo proposto está ligado a gaps identificados no Dia 6.
- [x] Gaps críticos não priorizados são declarados como adiados.
- [x] A resposta contém a tabela final
  `Gap atacado | Semana | Como vou comprovar`.
- [x] A resposta termina com uma pergunta de reflexão.
- [x] A resposta não inventa competências, experiência profissional ou nível de
  inglês.

## Evidências a registrar

- Prompt executável: `../../../prompts/prompt-dia-07.md`
- Resultado: `../resultado-modelo.md`
- Documentação do desafio: `../../../desafios/dia-07-mega-prompt.md`

## Limites

- Não alterar os desafios dos Dias 1 a 6 para facilitar a composição.
- Não substituir a vaga-alvo ou o relatório de gaps do Dia 6 sem nova execução.
- Não transformar o Tutor em aplicação, agente, RAG ou integração de API.
- Não fazer commit, push, pull request ou merge durante esta tarefa.
