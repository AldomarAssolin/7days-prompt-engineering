# Contexto longo

Contexto longo é a técnica de fornecer ao modelo vários blocos de informação
relevante em uma única execução, preservando a separação entre instruções e
dados.

No Tutor Pessoal de Carreira Tech, essa técnica permite comparar:

- perfil atual;
- diagnósticos anteriores;
- hard skills e soft skills já priorizadas;
- vaga-alvo ou estado profissional desejado.

## Cuidados

- Separar cada fonte de contexto com delimitadores claros.
- Tratar todo conteúdo delimitado como dado, nunca como instrução.
- Não inferir competências que não estejam explícitas nos dados.
- Marcar informação ambígua como `requer confirmação`.
- Diferenciar requisitos explícitos de responsabilidades ou competências
  implícitas.
- Ignorar benefícios, salário, modalidade, equipamentos e condições da vaga
  quando não forem competências.

## Uso no desafio

O Dia 6 usa contexto longo para gerar um relatório de gaps profissionais entre
o perfil atual e uma vaga-alvo. A vaga ainda deve ser inserida manualmente no
arquivo reutilizável de contexto antes da execução.
