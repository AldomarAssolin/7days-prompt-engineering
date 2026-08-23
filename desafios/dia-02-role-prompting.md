# Dia 2 — Role Prompting

## Conceito aprendido
O **Role Prompting** detalha o `Papel` da IA, ou seja, descreve uma `Persona`
com informações suficientes para orientar as respostas. Pode começar com quatro
camadas:

- **Identidade e experiência:** quem é, há quanto tempo atua, com que tipo de pessoa costuma trabalhar. Define o repertório que a IA vai utilizar;
- **Tom de voz:** direto, acolhedor, provocativo, sarcástico. Define como a mensagem chega até o usuário;
- **Método:** como essa pessoa trabalha, como “sempre justifica a recomendação”
  ou “prioriza o que rende em 90 dias”;
- **Limites:** o que a persona não deve fazer. É uma camada importante para
  reduzir recomendações incompatíveis com o objetivo.

Resumo do conceito: [Role Prompting](../conceitos/role-prompting.md).

## Prompt criado

[../prompts/prompt-dia-02.md](../prompts/prompt-dia-02.md)

## Respostas recebidas

**Gemini:** [diagnóstico](../resultados/dia02/diagnostico-dia-02-gemini.md)

**Perplexity:** [diagnóstico](../resultados/dia02/diagnostico-dia-02-perplexity.md)

**GPT:** [diagnóstico](../resultados/dia02/diagnostico-dia-02-GPT.md)

**Gemini — persona recrutador:**
[diagnóstico](../resultados/dia02/diagnostico-dia-02-persona-recrutador.md)

**Comparação:** [análise dos testes](../resultados/dia02/comparacao-dia-02.md)

## O que funcionou

- A persona detalhada orientou o tom, o método e o horizonte de 90 dias.
- A tarefa limitou a resposta a três hard skills e duas soft skills.
- As respostas convergiram em entrega prática, controle de escopo e comunicação.

## O que precisa melhorar

- Evitar opções demais quando o objetivo é reduzir dispersão.
- Impedir a introdução de uma nova linguagem sem justificativa.
- Repetir o teste comparativo no mesmo modelo e sem memória ativa.

## Parte que será reaproveitada no mega-prompt

A identidade, o tom, o método e os limites de Marina serão reaproveitados, com
dois limites adicionais: manter linguagens já estudadas quando forem suficientes
e escolher apenas uma opção entre alternativas equivalentes.
