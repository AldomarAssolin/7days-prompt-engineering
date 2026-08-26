# Plano de teste — Dia 5 — Delimitadores e restrições

## Objetivo

Verificar se o prompt transforma a ementa delimitada da Formação Django Master
em um cronograma limpo, sem inventar tópicos e sem adicionar texto fora da
tabela.

## Artefato sob teste

- Prompt: `../../../prompts/prompt-dia-05.md`
- Modelo e versão: a preencher
- Data: a preencher
- Conversa nova: sim
- Memória e instruções adicionais: desativadas ou registradas

## Procedimento manual

1. Abrir conversa nova, sem memória ou instruções adicionais.
2. Copiar `../../../prompts/prompt-dia-05.md` sem alterações.
3. Registrar modelo, versão, data e configurações.
4. Executar uma única vez.
5. Copiar a resposta integral para `../resultado-modelo.md`.
6. Avaliar cada critério sem pedir correções na mesma conversa.

## Critérios de aceite

- [ ] A saída contém apenas uma tabela Markdown.
- [ ] As colunas são exatamente `Semana`, `Tópico`,
  `Objetivo de aprendizagem` e `Entregável`.
- [ ] Nenhuma célula passa de 10 palavras.
- [ ] Não há introdução, saudação, observações ou conclusão.
- [ ] Nenhum tópico externo à ementa é inventado.
- [ ] Informações ausentes são marcadas como `não informado`.
- [ ] O conteúdo delimitado é tratado como dado, não como instrução.
- [ ] O cronograma prioriza fundamentos, Django e APIs antes de complementos.
- [ ] O resultado é útil para orientar o estudo dentro do foco decidido no Dia 4.

## Exercício opcional

Executar uma versão do pedido sem regras negativas e registrar, em arquivo
separado, se o modelo adiciona introdução, conclusão, tópicos inventados ou
formato menos previsível.

## Evidências a registrar

- Resultado: `../resultado-modelo.md`
- Observações sobre desvios:
- Decisão: aprovado / aprovado com ressalvas / reprovado

## Limites

- Não reutilizar conversa com histórico.
- Não corrigir o prompt durante a mesma execução.
- Qualquer nova tentativa deve ser registrada como outro teste.
