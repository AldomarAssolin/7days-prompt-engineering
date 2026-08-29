# Dia 7 — Mega-prompt

## Conceito

O Dia 7 aplica composição de prompts. Em vez de criar uma instrução isolada, o
desafio reúne os blocos produzidos nos Dias 1 a 6 em um Mega-Prompt
reutilizável para atuar como Tutor Pessoal de Carreira Tech.

A composição segue esta ordem:

1. Persona.
2. Contexto.
3. Base de conhecimento.
4. Lógica de raciocínio.
5. Padrão de saída.
6. Restrições.
7. Tarefa.

## Contexto

O Dia 7 depende dos artefatos anteriores e não refaz os desafios já concluídos.
A matriz de reutilização é:

| Dia | Artefato reutilizado | Bloco no Mega-Prompt | Situação |
| --- | --- | --- | --- |
| 1 | `contexto/perfil-base.md` e `prompts/prompt-dia-01.md` | Contexto sobre mim | Reutilizado sem alteração. |
| 2 | `contexto/persona.md` e `prompts/prompt-dia-02.md` | Persona | Reutilizado com limites já consolidados. |
| 3 | `prompts/prompt-dia-03.md` e `resultados/dia03/resultado-modelo.md` | Padrão de saída semanal | Adaptado para 4 semanas e fim de semana. |
| 4 | `prompts/prompt-dia-04.md` e `resultados/dia04/resultado-modelo.md` | Lógica de raciocínio | Adaptado para cruzar gaps, tempo e escopo. |
| 5 | `prompts/prompt-dia-05.md` | Restrições e delimitadores | Reutilizado para tratar fontes como dados. |
| 6 | `contexto/vagas/bairesdev-python-jr-2026-08-27.md` e `resultados/dia06/resultado-complementar-ajustes-dia-06.md` | Base de conhecimento | Reutilizada como vaga-alvo e relatório de gaps. |

Lacunas e incompatibilidades identificadas:

- O nível de inglês não está informado no perfil, então não pode ser tratado
  como competência existente.
- A vaga exige 1 ano de experiência com Python, mas o perfil informa apenas
  estudo e necessidade de consolidação por projetos.
- O Dia 3 planejava somente dias úteis; para o Dia 7, o padrão foi estendido
  para incluir as 4 horas de fim de semana declaradas no perfil.
- O limite de no máximo 3 tecnologias ou temas obriga a adiar pelo menos um gap
  crítico. O inglês foi registrado como adiado no resultado por falta de dados e
  por não caber junto dos três temas priorizados.

## Desafio

Construir um Mega-Prompt denominado Tutor Pessoal de Carreira Tech usando os
artefatos dos seis dias anteriores e gerar um PDI executável de 30 dias.

Critérios de aceite:

- O Mega-Prompt possui os blocos `PERSONA`, `CONTEXTO`, `BASE DE CONHECIMENTO`,
  `LÓGICA DE RACIOCÍNIO`, `PADRÃO DE SAÍDA`, `RESTRIÇÕES` e `TAREFA`.
- Os blocos reutilizam os artefatos dos Dias 1 a 6.
- A vaga-alvo e o relatório de gaps são tratados como dados delimitados.
- O PDI tem exatamente 30 dias, organizado em 4 semanas com dois dias extras de
  fechamento quando necessário.
- A resposta começa com diagnóstico de no máximo 5 linhas.
- Cada semana segue o padrão de plano semanal derivado do Dia 3.
- Cada semana termina com entregável verificável.
- Todo conteúdo proposto está ligado a gaps identificados no Dia 6.
- O plano usa no máximo 3 tecnologias ou temas.
- Gaps críticos que não couberem em 30 dias são declarados explicitamente.
- A resposta contém a tabela final `Gap atacado | Semana | Como vou comprovar`.
- A resposta termina com uma pergunta de reflexão.
- O Mega-Prompt foi salvo em Markdown versionável.

Fora do escopo:

- Refazer os desafios dos Dias 1 a 6.
- Alterar a vaga-alvo usada no Dia 6.
- Inventar competências, nível de inglês, experiência profissional ou domínio
  de ferramentas.
- Criar plano maior que 30 dias.
- Introduzir mais de 3 tecnologias ou temas.
- Criar aplicação, agente autônomo, RAG, integração de API ou memória
  persistente.
- Fazer commit, push, pull request ou merge.

## Prompt

O Mega-Prompt executável está em
[`../prompts/prompt-dia-07.md`](../prompts/prompt-dia-07.md).

## Resultado

O resultado da execução controlada está em
[`../resultados/dia07/resultado-modelo.md`](../resultados/dia07/resultado-modelo.md).

Resumo da execução:

- Modelo e versão: Codex / GPT-5.
- Data: 29/08/2026.
- Conversa nova: não; execução registrada nesta tarefa.
- Prompt usado: `../../prompts/prompt-dia-07.md`.
- Decisão: aprovado com ressalva quanto ao isolamento da conversa.

## Template

Estrutura reutilizável do Mega-Prompt:

```text
# 1. PERSONA
{{persona_mentor}}

# 2. CONTEXTO SOBRE MIM
<PERFIL_BASE>
"""
{{perfil_base}}
"""
</PERFIL_BASE>

# 3. BASE DE CONHECIMENTO
<VAGA_ALVO>
"""
{{vaga_alvo}}
"""
</VAGA_ALVO>

<RELATORIO_DE_GAPS>
"""
{{relatorio_de_gaps}}
"""
</RELATORIO_DE_GAPS>

# 4. LÓGICA DE RACIOCÍNIO
{{sequencia_de_analise}}

# 5. PADRÃO DE SAÍDA
{{exemplo_ou_modelo_de_saida}}

# 6. RESTRIÇÕES
{{regras_de_formato_escopo_e_delimitadores}}

# 7. TAREFA
{{tarefa_final}}
```
