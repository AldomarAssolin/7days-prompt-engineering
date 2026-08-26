# Delimitadores e restrições

Delimitadores são marcadores usados para separar instruções de dados. Eles
indicam ao modelo qual parte do prompt deve orientar a resposta e qual parte
deve apenas ser processada.

Exemplos de delimitadores:

- aspas triplas: `"""`;
- três traços: `---`;
- tags: `<ementa>...</ementa>`.

Essa separação reduz ambiguidade quando o prompt contém textos longos, ementas,
editais, índices, transcrições ou qualquer conteúdo que possa incluir frases com
aparência de comando.

Restrições são regras explícitas sobre a saída. Elas podem definir formato,
extensão e comportamentos proibidos.

Tipos úteis de restrição:

- formato: tabela Markdown, lista numerada, JSON ou blocos fixos;
- extensão: limite de linhas, palavras ou itens;
- negativas: não incluir introdução, não inventar dados, não concluir fora do
  escopo;
- fallback: escrever `não informado` quando uma informação não existir.

No projeto do Tutor Pessoal de Carreira Tech, delimitadores e restrições serão
reaproveitados para transformar materiais externos em planos objetivos, sem que
a IA misture o conteúdo colado com novas instruções.
