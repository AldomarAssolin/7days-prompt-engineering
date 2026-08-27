# Plano de teste — Dia 6 — Contexto longo

## Objetivo

Verificar se o prompt compara o perfil atual com uma vaga-alvo sem inventar
competências, separando requisitos já evidenciados de gaps críticos e
secundários.

## Artefato sob teste

- Prompt: `../../../prompts/prompt-dia-06.md`
- Contexto de vaga: `../../../contexto/vaga-alvo-dia-06.md`
- Modelo e versão: a preencher
- Data: a preencher
- Conversa nova: sim
- Memória e instruções adicionais: desativadas ou registradas

## Pré-condição

A vaga-alvo deve estar preenchida em
`../../../contexto/vaga-alvo-dia-06.md`. Não executar este teste com o
placeholder original.

## Procedimento manual

1. Preencher `../../../contexto/vaga-alvo-dia-06.md` com a vaga real.
2. Abrir conversa nova, sem memória ou instruções adicionais.
3. Copiar `../../../prompts/prompt-dia-06.md`.
4. Substituir os quatro placeholders pelos conteúdos integrais indicados.
5. Executar uma única vez.
6. Copiar a resposta integral para `../resultado-modelo.md`.
7. Avaliar cada critério sem pedir correções na mesma conversa.

## Critérios de aceite

- [ ] A saída contém somente as seções `JÁ TENHO`, `GAPS CRÍTICOS` e
  `GAPS SECUNDÁRIOS`.
- [ ] Cada seção contém apenas uma tabela Markdown.
- [ ] Todas as tabelas usam exatamente as colunas `Requisito`, `Situação` e
  `Evidência / Observação`.
- [ ] Não há introdução, saudação, observações fora das tabelas ou conclusão.
- [ ] O modelo não infere habilidades sem evidência explícita.
- [ ] Informações ambíguas aparecem como `requer confirmação`.
- [ ] Requisitos explícitos da vaga são distinguidos de responsabilidades ou
  competências implícitas quando aplicável.
- [ ] Benefícios e condições não relacionados a competências são ignorados.
- [ ] Conhecimentos transferíveis aparecem apenas como observação, sem comprovar
  o requisito específico.
- [ ] `GAPS CRÍTICOS` está ordenado por impacto.

## Evidências a registrar

- Resultado: `../resultado-modelo.md`
- Observações sobre desvios:
- Decisão: aprovado / aprovado com ressalvas / reprovado

## Limites

- Não executar o prompt antes de inserir uma vaga real.
- Não corrigir o prompt durante a mesma execução.
- Qualquer nova tentativa deve ser registrada como outro teste.
