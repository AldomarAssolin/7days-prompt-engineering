# Dia 1 — Papel, Tarefa e Contexto (PTC)

## Conceito aprendido

Um prompt PTC informa:

- **Papel:** quem a IA deve representar, definindo perspectiva, linguagem e
  nível técnico.
- **Tarefa:** o resultado que a IA deve produzir, descrito com verbos e critérios
  objetivos.
- **Contexto:** a situação, os conhecimentos, o objetivo, as limitações e as
  dificuldades da pessoa.

Quanto mais específico for o contexto, menor será a chance de receber uma
resposta genérica.

## Prompt criado

```text
PAPEL:

Você é um orientador de carreira em tecnologia, com experiência em ajudar
pessoas em início de jornada a entender onde estão e o que priorizar.
Sua linguagem é direta e acessível, sem jargões desnecessários.

TAREFA:

Faça um diagnóstico do meu momento atual de carreira e estudos.
Aponte 3 pontos fortes que eu já tenho, 3 lacunas que precisam de atenção
e 1 risco que eu provavelmente não estou enxergando.

CONTEXTO:

- Momento atual: trabalho na indústria e estou construindo uma transição
  gradual para atuar com tecnologia e soluções digitais.
- O que já estudei: Python, banco de dados, HTML, CSS e JavaScript. Preciso
  consolidar esses conhecimentos por meio de projetos completos.
- Objetivo: planejar, desenvolver, testar e publicar sites e pequenos sistemas
  web para construir o portfólio da Assolin Tecnologia e, futuramente, atender
  pequenos negócios.
- Tempo disponível: 1 hora por dia durante a semana e 4 horas no fim de semana,
  totalizando aproximadamente 9 horas semanais.
- Maior dificuldade: perco-me na quantidade de conteúdos e tecnologias e não
  sei o que estudar primeiro.
- Forma preferida de aprendizado: projetos pequenos e progressivos, combinando
  explicação, prática e revisão.
- Restrições: preciso evitar várias tecnologias simultaneamente e priorizar o
  que estiver relacionado ao projeto atual.
```

## Resultado

### Diagnósticos

**ChatGPT**: 
[`../resultados/diagnostico-dia-01-GPT.md`](../resultados/diagnostico-dia-01-GPT.md).

**Gemini**: 
[`../resultados/diagnostico-dia-01-gemini.md`](../resultados/diagnostico-dia-01-gemini.md).

**Claude**: 
[`../resultados/diagnostico-dia-01-claude.md`](../resultados/diagnostico-dia-01-claude.md).

**Perplexity — prompt genérico**:
[`../resultados/diagnostico-dia-01-prompt-generico-perplexity.md`](../resultados/diagnostico-dia-01-prompt-generico-perplexity.md).

**Síntese comparativa**:
[`../resultados/comparacao-dia-01.md`](../resultados/comparacao-dia-01.md).

## O que funcionou

- O papel definiu uma orientação apropriada para quem está em transição.
- A tarefa exigiu uma estrutura verificável: 3 forças, 3 lacunas e 1 risco.
- O tempo semanal permitiu uma recomendação compatível com a rotina real.
- O objetivo passou a conectar os estudos à Assolin Tecnologia e a projetos
  para pequenos negócios.

## O que precisa melhorar

- Identificar, em um próximo passo, qual será o primeiro projeto concreto.
- Registrar o nível real de autonomia em cada tecnologia estudada.
- Definir um critério de conclusão para o primeiro projeto publicado.

## Parte que será reaproveitada no mega-prompt

O bloco `CONTEXTO` será a base permanente do Tutor Pessoal de Carreira Tech.
Ele poderá ser atualizado sempre que um projeto for concluído ou a prioridade
profissional mudar.

## Comparação com o prompt genérico

O exercício opcional foi realizado no Perplexity, em uma conversa sem o Perfil
Base de Contexto, usando somente o prompt:

```text
Faça um diagnóstico da minha carreira em tecnologia.
```

A resposta genérica não conseguiu diagnosticar minha situação pessoal. Em vez
disso, apresentou tendências amplas do mercado de tecnologia e solicitou dados
como cargo, experiência, formação, conhecimentos, objetivo e dificuldade atual.

Já as respostas ao prompt PTC identificaram de forma consistente:

- minha transição gradual da indústria para a tecnologia;
- a necessidade de integrar Python, banco de dados, HTML, CSS e JavaScript;
- a importância de concluir e publicar projetos para a Assolin Tecnologia;
- um plano compatível com aproximadamente nove horas semanais;
- o risco de dispersão e de ampliar o escopo antes da primeira entrega.

### Conclusão do experimento

O teste confirmou que o modelo não consegue produzir um diagnóstico pessoal
apenas com um pedido genérico. O Papel orientou a perspectiva da resposta, a
Tarefa definiu critérios verificáveis e o Contexto forneceu os dados necessários
para transformar recomendações gerais em orientações aplicáveis à minha
realidade.
