# Plano de teste — Dia 6 — Contexto longo

## Objetivo

Verificar se o prompt compara o perfil atual com uma vaga-alvo sem inventar
competências, separando requisitos já evidenciados de gaps críticos e
secundários.

## Artefato sob teste

- Template do prompt: `../../../prompts/prompt-dia-06.md`
- Prompt final da primeira execução: `../prompt-final-2026-08-27-gpt-5-5.md`
- Prompt final complementar: `../prompt-final-complementar-2026-08-29-ajustes-dia-06.md`
- Contexto de vaga: `../../../contexto/vagas/bairesdev-python-jr-2026-08-27.md`
- Modelo e versão: a preencher
- Data: a preencher
- Conversa nova: sim
- Memória e instruções adicionais: desativadas ou registradas

## Pré-condição

A vaga-alvo deve estar preenchida em
`../../../contexto/vagas/bairesdev-python-jr-2026-08-27.md`. Não executar este teste com o
placeholder original.

## Procedimento manual

1. Preencher um arquivo em `../../../contexto/vagas/` com a vaga real.
2. Copiar `../../../prompts/prompt-dia-06.md` para um arquivo de prompt final.
3. Substituir os placeholders pelos conteúdos integrais indicados.
4. Registrar as fontes usadas em um manifesto de contexto.
5. Abrir conversa nova, sem memória ou instruções adicionais.
6. Executar o prompt final uma única vez.
7. Copiar a resposta integral para `../resultado-modelo.md`.
8. Avaliar cada critério sem pedir correções na mesma conversa.
9. Caso a revisão identifique falha no prompt de origem, registrar uma execução
   complementar separada, preservando a primeira execução com ressalvas.

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
- [ ] `JÁ TENHO` não contém itens parciais, complementares, transferíveis ou
  classificados como `requer confirmação`.

## Evidências a registrar

- Resultado: `../resultado-modelo.md`
- Resultado complementar: `../resultado-complementar-ajustes-dia-06.md`
- Manifesto de contexto: `../contexto-manifest.md`
- Observações sobre desvios: primeira execução com ressalvas; execução
  complementar registrada após ajustes mínimos no prompt.
- Decisão: primeira execução aprovada com ressalvas; execução complementar
  consolidada.

## Limites

- Não executar o prompt antes de inserir uma vaga real.
- Não corrigir o prompt durante a mesma execução.
- Qualquer nova tentativa deve ser registrada como outro teste.
