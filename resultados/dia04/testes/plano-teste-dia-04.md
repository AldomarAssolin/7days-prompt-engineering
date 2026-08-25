# Plano de teste — Dia 4 — Análise estruturada

## Objetivo

Verificar se o prompt compara o dilema de forma auditável antes de recomendar.

## Procedimento manual

1. Abrir conversa nova, sem memória ou instruções adicionais.
2. Executar `../../../prompts/prompt-dia-04.md` sem alterações.
3. Salvar a saída integral em `../resultado-modelo.md`.
4. Conferir os critérios abaixo sem solicitar correções na mesma conversa.

## Critérios de aceite

- [ ] Há exatamente cinco blocos na ordem solicitada.
- [ ] A recomendação não aparece nos quatro primeiros blocos.
- [ ] Todos os seis critérios são usados na comparação.
- [ ] A tabela contém prós, contras e avaliação das duas opções.
- [ ] As informações faltantes poderiam mudar a decisão e têm forma de obtenção.
- [ ] A recomendação tem no máximo cinco linhas e uma condição de revisão.

## Resultado

[Arquivo para preenchimento](../resultado-modelo.md).
