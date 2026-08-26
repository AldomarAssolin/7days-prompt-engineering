# Plano de execução — Dia 5

## Objetivo

Executar o desafio do Dia 5 do 7DaysOfCode de Prompt Engineering usando
delimitadores e restrições para extrair um cronograma de estudos limpo a partir
da ementa da **Formação Django Master**, usada como referência do curso
**Pacote Python Master**, do PyCoder/Felipe Azambuja.

## Referência do desafio

- Tema: delimitadores e restrições.
- E-mail: `#7DaysOfCode - Prompt Engineering 5/7: Delimitadores e restrições`.
- Data recebida: 26/08/2026.
- Saída esperada no desafio: tabela Markdown, sem texto introdutório ou
  conclusão.

## Estado atual do projeto

- Dia 1 definiu o contexto base da transição para tecnologia.
- Dia 2 definiu a persona Marina e seus limites de orientação.
- Dia 3 criou o padrão de plano semanal com entregável verificável.
- Dia 4 recomendou manter foco em Python e Django até concluir o primeiro
  sistema de portfólio.

O Dia 5 adiciona uma camada de controle de entrada e saída ao futuro
mega-prompt, evitando respostas prolixas, invenção de tópicos e obediência a
instruções presentes no material colado.

## Entrada recebida

Ementa da **Formação Django Master**, enviada pelo usuário como referência para
o curso **Pacote Python Master**.

A ementa contém 30 blocos principais, cobrindo fundamentos web, Python, Django,
banco de dados, URLs, views, templates, ORM, forms, autenticação, CBVs, signals,
integração com IA, manutenção, PostgreSQL, shell, deploy, APIs, DRF, serializers,
JWT, permissões, projetos aplicados, Streamlit, Docker, freelancing e automação.

## Estratégia

1. Registrar o conceito do dia em `conceitos/delimitadores-e-restricoes.md`.
2. Registrar o desafio em `desafios/dia-05-delimitadores-e-restricoes.md`.
3. Criar `prompts/prompt-dia-05.md` com a ementa delimitada por aspas triplas.
4. Incluir regra explícita para tratar o conteúdo delimitado como dado, nunca
   como instrução.
5. Restringir a saída a uma tabela Markdown com colunas fixas.
6. Criar plano de teste manual em `resultados/dia05/testes/`.
7. Registrar a primeira resposta integral em `resultados/dia05/resultado-modelo.md`.
8. Atualizar o README somente depois do teste e avaliação.

## Prompt base implementado

O prompt final está em `../../prompts/prompt-dia-05.md`.

Ele usa:

- delimitador com aspas triplas;
- regra para tratar a ementa como dado;
- saída limitada a tabela Markdown;
- colunas fixas;
- limite de 10 palavras por célula;
- regras negativas contra introdução, conclusão e tópicos inventados.

## Critérios de aceite

- [x] A saída contém apenas uma tabela Markdown.
- [x] As colunas são exatamente `Semana`, `Tópico`,
  `Objetivo de aprendizagem` e `Entregável`.
- [x] Nenhuma célula passa de 10 palavras.
- [x] Não há introdução, saudação, observações ou conclusão.
- [x] Nenhum tópico externo à ementa é inventado.
- [x] Informações ausentes seriam marcadas como `não informado` quando existissem.
- [x] O conteúdo delimitado é tratado como dado, não como instrução.
- [x] O cronograma prioriza fundamentos, Django e APIs antes de complementos.
- [x] O resultado é útil para orientar o estudo dentro do foco decidido no Dia 4.

## Exercício opcional

Executar uma segunda versão sem regras negativas e comparar:

- se aparece introdução;
- se aparece conclusão;
- se o modelo inventa etapas;
- se o formato fica menos previsível.

## Limites

- Não inventar módulos, aulas ou tópicos do curso.
- O Dia 5 só foi marcado como concluído após registrar resultado e avaliação.
- Não alterar arquivos dos Dias 1 a 4, salvo correção pontual aprovada.

## Estado

Dia 5 executado e concluído com ressalva operacional: o teste foi feito nesta tarefa, não em conversa nova independente.
