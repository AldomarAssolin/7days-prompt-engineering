## 1. Plano de hard skills

### 1º — Desenvolvimento backend com Python e Django

**Prioridade:** essencial.

Consolide Python dentro do Django, aprendendo:

- rotas, views e templates;
- formulários e validação;
- autenticação;
- operações CRUD;
- organização básica do projeto.

**Por que vem primeiro:** seu objetivo não é apenas criar páginas, mas entregar pequenos sistemas. O Django reúne várias necessidades profissionais em uma estrutura só, evitando que você precise escolher e integrar muitas ferramentas agora.

**Projeto prático:** sistema de cadastro de clientes, serviços e solicitações para um pequeno negócio.

> Use Django gratuitamente. Não acrescente outro framework backend, como Flask ou FastAPI, durante estes 90 dias.

### 2º — Banco de dados aplicado com PostgreSQL

**Prioridade:** essencial.

Desenvolva competência em:

- modelagem de tabelas e relacionamentos;
- consultas SQL fundamentais;
- integração do banco com o Django;
- migrations;
- validação, atualização e exclusão segura de dados.

**Por que vem em segundo:** sistemas úteis para pequenos negócios precisam armazenar clientes, pedidos, serviços e status corretamente. Entender os dados evita criar aplicações que funcionam apenas como demonstração visual.

**Projeto prático:** evoluir o sistema anterior com relacionamentos, como:

```text
Cliente → várias solicitações → cada solicitação possui serviço e status
```

Você pode usar PostgreSQL localmente ou em uma plataforma com plano gratuito. Para o início do projeto, o SQLite incluído no Django também é uma alternativa gratuita e mais simples.

### 3º — Frontend responsivo com HTML, CSS e JavaScript

**Prioridade:** essencial, mas com escopo controlado.

Consolide:

- HTML semântico;
- layouts responsivos;
- formulários claros;
- manipulação básica do DOM;
- feedback de erros, carregamento e sucesso.

**Por que vem em terceiro:** seus sistemas precisam ser utilizáveis no celular e transmitir confiança aos futuros clientes. Porém, React, Vue ou outro framework agora aumentaria a dispersão sem ser necessário para os primeiros projetos.

**Projeto prático:** criar uma interface responsiva para o sistema e uma landing page da Assolin Tecnologia.

Use CSS puro ou Bootstrap, ambos gratuitos. Escolha apenas um durante o ciclo.

### Bom ter depois dos 90 dias

- APIs REST;
- React ou Vue;
- Docker;
- testes avançados;
- serviços de nuvem mais complexos.

Git, testes básicos e publicação entram no fluxo dos projetos, mas não como novas frentes independentes de estudo. Aprenda somente o necessário para versionar, verificar e colocar cada entrega no ar.

## 2. Plano de soft skills

### 1º — Priorização e controle de escopo

**Por que é crítica:** sua dificuldade declarada é decidir o que estudar. Sem um escopo fechado, cada conteúdo novo parece necessário e os projetos não chegam à publicação.

**Ação concreta:** todo domingo, reserve 20 minutos para definir uma única entrega verificável da semana, por exemplo:

> “Até domingo, o usuário poderá cadastrar e listar clientes.”

Crie também uma lista chamada **Depois dos 90 dias**. Toda tecnologia ou ideia que não seja necessária para a entrega atual vai para essa lista, sem pesquisa adicional naquela semana.

### 2º — Comunicação orientada ao problema do cliente

**Por que é crítica:** pequenos negócios não compram Django, PostgreSQL ou JavaScript. Eles procuram redução de trabalho manual, organização e mais oportunidades de venda. Seu portfólio precisa demonstrar esse entendimento.

**Ação concreta:** ao concluir cada funcionalidade, grave uma apresentação de até três minutos respondendo:

1. Qual problema do negócio ela resolve?
2. Como o usuário utiliza a solução?
3. Qual resultado ela pode gerar?
4. O que ainda está fora do escopo?