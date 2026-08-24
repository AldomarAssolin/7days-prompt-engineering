# 7DaysOfCode — Prompt Engineering 3/7

## Atividade

Aplicar **Few-Shot Prompting** para transformar a prioridade nº 1 da lista de hard skills produzida no Dia 2 em um plano de estudos de uma semana. O prompt deve fornecer de 2 a 4 exemplos de entrada e saída para ensinar à IA o padrão desejado — estrutura, extensão e tom — sem induzi-la a copiar o conteúdo dos exemplos.

## Objetivo

Produzir, com a persona da Marina criada no Dia 2 e o Perfil Base de Contexto do Dia 1, uma semana de estudos para a hard skill prioritária. A resposta deve repetir com consistência o formato dos exemplos: título da semana, uma meta, cinco atividades diárias (segunda a sexta) e um entregável final.

## Critérios de conclusão

- A persona da Marina contém experiência declarada, método explícito e pelo menos duas regras negativas.
- A prioridade nº 1 de hard skills e o Perfil Base de Contexto estão inseridos no prompt.
- Há entre 2 e 4 exemplos, usando temas diferentes da hard skill escolhida.
- Todos os exemplos seguem a mesma estrutura, extensão e tom.
- A resposta final contém título, meta, cinco dias de estudo e entregável.
- O plano é adequado ao contexto e à disponibilidade informados no Dia 1.
- O prompt e seus exemplos estão salvos para reutilização nos próximos dias e no projeto do Dia 7.

## Tarefas

- [ ] Recuperar o Perfil Base de Contexto criado no Dia 1.
- [ ] Recuperar a persona da Marina e a lista priorizada de hard skills do Dia 2.
- [ ] Validar a persona: experiência, método e duas regras negativas.
- [ ] Identificar e registrar a prioridade nº 1 da lista de hard skills.
- [ ] Definir o padrão do plano: título, meta, segunda a sexta e entregável.
- [ ] Preparar de 2 a 4 exemplos de entrada e saída sobre temas diferentes da prioridade escolhida.
- [ ] Montar o prompt Few-Shot com PAPEL, TAREFA, EXEMPLOS, ENTRADA, CONTEXTO e SAÍDA.
- [ ] Executar o prompt e gerar a semana de estudos.
- [ ] Conferir se a saída preserva exatamente a estrutura e o número de linhas dos exemplos.
- [ ] Se o formato variar, acrescentar: “Mantenha exatamente a estrutura dos exemplos, inclusive o número de linhas.”
- [ ] Revisar se a meta é verificável, as atividades são executáveis e o entregável é concreto.
- [ ] Salvar o prompt, os exemplos e o plano final para reutilização no Dia 7.
- [ ] Opcional: publicar o resultado no GitHub e compartilhar com as hashtags #7DaysOfCode e #feedback7DoC.

## Modelo de prompt

```text
PAPEL:
[cole aqui a persona da Marina, do Dia 2]

TAREFA:
Abaixo estão exemplos de como eu quero que um plano de estudos semanal seja escrito. Aprenda o PADRÃO (estrutura, extensão e tom), não o conteúdo. Depois monte a minha próxima semana seguindo exatamente esse padrão.

EXEMPLO 1
[entrada e saída sobre um tema diferente]

EXEMPLO 2
[entrada e saída sobre outro tema diferente]

AGORA É A SUA VEZ:
Entrada: [prioridade nº 1 da lista de hard skills do Dia 2]
Contexto: [Perfil Base de Contexto do Dia 1]

Saída:
Mantenha exatamente a estrutura dos exemplos, inclusive o número de linhas.
```
