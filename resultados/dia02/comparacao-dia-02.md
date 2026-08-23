# Comparação do Dia 2 — Role Prompting

## Objetivo do experimento

Avaliar como a definição detalhada do papel influencia prioridades, linguagem,
método e limites da resposta. O prompt-base usa **Marina**, mentora sênior que
orienta pessoas em transição de carreira, prioriza resultados em 90 dias e
limita o número de tecnologias. O teste comparativo troca somente a persona por
um **recrutador tech com dez anos de experiência**, mantendo tarefa e contexto.

## Testes analisados

- [Gemini — persona Marina](diagnostico-dia-02-gemini.md)
- [GPT — persona Marina](diagnostico-dia-02-GPT.md)
- [Perplexity — persona Marina](diagnostico-dia-02-perplexity.md)
- [Gemini — persona recrutador](diagnostico-dia-02-persona-recrutador.md)

O contraste mais controlado é entre as duas respostas do Gemini, pois o modelo,
a tarefa e o contexto permanecem equivalentes. GPT e Perplexity ajudam a medir
a consistência do prompt-base entre modelos, mas não isolam o efeito da persona.

## Comparação controlada: mentora versus recrutador

| Critério | Marina — mentora | Recrutador tech |
|---|---|---|
| Perspectiva principal | Aprendizado progressivo e entrega para clientes | Evidência de autonomia para recrutadores e clientes |
| Tom | Acolhedor, direto e preventivo | Avaliativo, direto e orientado à empregabilidade |
| Prioridade técnica | Backend/API, dados e publicação | Backend/dados, frontend e Git/deploy |
| Critério de sucesso | Colocar um fluxo mínimo no ar em 90 dias | Produzir aplicação pública e portfólio verificável |
| Tratamento da dispersão | Cortar 50% do escopo e manter um fluxo principal | Limitar o projeto a três funcionalidades |
| Comunicação | Explicar dor, processo eliminado e uso | Explicar problema, arquitetura e forma de testar |
| Aderência aos limites | Alta | Parcial: preserva foco, mas combina mais ferramentas na terceira prioridade |

## Efeito observado da persona

A troca de papel não alterou radicalmente as tecnologias porque tarefa e
contexto já restringiam bastante o problema. Ela alterou principalmente o
**critério usado para justificar as recomendações**:

- A mentora enfatizou carga de estudo, prevenção de frustração, escopo mínimo e
  valor entregue ao pequeno negócio.
- O recrutador enfatizou comprovação de autonomia, decisões de arquitetura,
  repositório organizado e aplicação pública como evidência profissional.

Isso mostra que o papel funciona como uma lente de decisão. Entretanto, quando
a tarefa e o contexto são muito específicos, trocar apenas uma frase de persona
gera diferenças de ênfase, não necessariamente planos opostos.

## Consenso entre as respostas com a persona Marina

As respostas de Gemini, GPT e Perplexity convergiram em quatro pontos:

1. Consolidar conhecimentos por meio de um projeto completo, não de cursos
   isolados.
2. Trabalhar com no máximo três frentes técnicas durante o ciclo.
3. Praticar priorização e controle de escopo como soft skill central.
4. Comunicar o problema resolvido e transformar o projeto em evidência pública.

## Divergências técnicas

| Modelo | Três prioridades propostas | Observação |
|---|---|---|
| Gemini | Python com Flask/FastAPI, banco de dados e deploy | Valoriza publicação, mas oferece escolhas demais entre frameworks e ferramentas. |
| GPT | Django, PostgreSQL e frontend fundamental | É o plano mais integrado e mais fiel ao limite de uma stack fixa. |
| Perplexity | Frontend, Node.js e Git/workflow | Introduz Node.js apesar do conhecimento prévio em Python, aumentando a dispersão que o papel deveria evitar. |

As divergências mostram que a persona controlou bem o método e o tom, mas não
foi suficiente para fixar uma stack. Para obter recomendações tecnicamente mais
consistentes, o mega-prompt deverá informar se novas linguagens podem ser
introduzidas e como desempatar alternativas equivalentes.

## Avaliação de aderência ao prompt-base

- **GPT:** maior aderência. Justificou prioridades, separou essencial de “bom ter
  depois”, limitou as frentes e apresentou alternativas gratuitas.
- **Gemini:** boa aderência. Entregou ações concretas e foco em 90 dias, mas
  apresentou Flask ou FastAPI, PostgreSQL ou SQLite, Postman ou Thunder Client e
  várias plataformas de deploy, criando escolhas que podem alimentar dispersão.
- **Perplexity:** aderência parcial. Foi conciso e respeitou a quantidade pedida,
  porém recomendou Node.js sem justificar o abandono de Python, não separou
  explicitamente o essencial do “bom ter depois” e aplicou pouco da identidade
  de Marina.
- **Gemini com recrutador:** boa resposta ao papel alternativo. A linguagem mudou
  para portfólio, avaliação e prova de autonomia, embora o resultado técnico
  continue próximo ao da mentora devido ao contexto compartilhado.

## Limitações do experimento

1. Os registros indicam memória ativa nos dois testes do Gemini. Isso pode ter
   influenciado a comparação e deve ser evitado em uma repetição controlada.
2. O arquivo do teste alternativo não reproduz integralmente o prompt executado;
   registra apenas a frase substituída e aponta para o prompt-base.
3. “Prompt genérico” é um nome impreciso: tarefa e contexto continuam
   detalhados. O nome correto seria **prompt com persona alternativa**.
4. Versões e modos diferentes dos modelos impedem atribuir todas as divergências
   exclusivamente ao Role Prompting.

## O que funcionou

- As quatro camadas da persona orientaram tom, justificativa, horizonte de tempo
  e controle de escopo.
- A tarefa determinou uma saída objetiva: três hard skills e duas soft skills.
- O limite de tecnologias conteve parte das recomendações expansivas.
- O contexto conectou os planos à Assolin Tecnologia e à disponibilidade de
  nove horas semanais.

## O que precisa melhorar

- Trocar o nome “prompt genérico” por “persona alternativa”.
- Repetir a comparação no mesmo modelo, em conversas novas e sem memória.
- Registrar o prompt alternativo completo, não apenas a frase modificada.
- Acrescentar o limite: “não introduza uma nova linguagem se uma já estudada
  atender ao objetivo; se introduzir, justifique a substituição”.
- Pedir uma única recomendação quando houver alternativas equivalentes, deixando
  as demais em “bom ter depois”.

## Parte que será reaproveitada no mega-prompt

```text
PAPEL:

Você é Marina, mentora sênior de tecnologia com 12 anos de experiência. Já foi
desenvolvedora, hoje lidera times e orienta pessoas em transição de carreira.
Seu tom é acolhedor e honesto: não romantiza o mercado nem promete atalhos.

MÉTODO:

- Justifique cada recomendação.
- Priorize resultados práticos alcançáveis em até 90 dias.
- Separe o essencial do que pode ficar para depois.

LIMITES:

- Não recomende mais de três frentes técnicas simultâneas.
- Não introduza uma nova linguagem quando uma já estudada atender ao objetivo.
- Quando houver alternativas equivalentes, escolha uma e explique o critério.
- Não use frases motivacionais vazias.
- Não sugira ferramenta paga sem indicar uma alternativa gratuita.
```

## Conclusão

O Role Prompting alterou com clareza a perspectiva e a justificativa das
respostas. A mentora raciocinou como alguém responsável por uma evolução
sustentável; o recrutador raciocinou como alguém procurando provas de prontidão
profissional. O experimento também mostrou que uma persona detalhada não elimina
ambiguidades técnicas: limites explícitos sobre stack e critérios de desempate
são necessários para impedir novas escolhas e preservar o foco.
