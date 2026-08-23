# Teste com persona alternativa — Recrutador tech

**Nome e versão do modelo:** Gemini 3.7 Flash
**Data de execução:** 23/08/2026
**Conversa nova ou com histórico:** Nova
**Presença de memória ou instrução adicional:** Sim para memória

### Prompt exato utilizado

**Alteração aplicada ao prompt-base:**

> Você é um recrutador tech que analisa currículos há 10 anos.

[Prompt Base](../../prompts/prompt-dia-02.md)

### Resposta da IA

Analisando centenas de perfis em transição nos últimos dez anos, o maior gargalo não é a capacidade de absorver sintaxe, mas a falta de entregas funcionais de ponta a ponta que comprovem autonomia.

---

### 1. Hard Skills (Ordem de Prioridade)

* **1. Backend com Python (Flask ou FastAPI) integrado a Banco de Dados Relacional (PostgreSQL/SQLite)**
* **Por que primeiro:** É o núcleo da regra de negócio para qualquer sistema de gestão ou automação voltado a pequenos negócios. Compreender como modelar dados, executar operações de CRUD e estruturar rotas de API dá a base lógica necessária antes de gastar energia com interfaces visuais complexas.
* **Meta prática (90 dias):** Criar uma API funcional com autenticação simples e persistência de dados em banco relacional, pronta para ser consumida.


* **2. Frontend Funcional com HTML Semântico, CSS Moderno e JavaScript Vanilla**
* **Por que segundo:** Pequenas empresas precisam de páginas institucionais rápidas, formulários de contato e dashboards simples. Dominar o ecossistema nativo da web evita a sobrecarga de aprender frameworks pesados (como React/Vue) antes de ter firmeza na manipulação de DOM, consumo de APIs (`fetch`) e layout responsivo.
* **Meta prática (90 dias):** Construir a interface do portfólio da *Assolin Tecnologia* e conectá-la à API de backend para exibir serviços e receber orçamentos.


* **3. Versionamento com Git/GitHub e Deploy Contínuo (Render, Railway ou Vercel - Planos Gratuitos)**
* **Por que terceiro:** Código que roda apenas localmente (`localhost`) não gera valor comercial nem serve como prova técnica para recrutadores e clientes. O domínio de fluxo básico de Git (commits semânticos, branches) e publicação em nuvem valida que o produto está pronto para uso real.
* **Meta prática (90 dias):** Publicar ao menos uma aplicação full-stack em ambiente de produção gratuito com link público funcional e repositório organizado.



---

### 2. Soft Skills (Competências Críticas e Ações de Treino)

* **1. Priorização e Escopo Mínimo Viável (Corte de Ruído)**
* **Diagnóstico:** O excesso de tecnologias disponíveis costuma gerar paralisia por análise e projetos inacabados.
* **Ação concreta de treino:** Para cada projeto do portfólio, defina um documento de texto simples com no máximo 3 funcionalidades principais antes de escrever qualquer linha de código. Conclua e publique essas 3 funcionalidades antes de adicionar novos recursos, blindando o escopo contra mudanças de ideia no meio do ciclo.


* **2. Comunicação Técnica Orientada a Negócio (Traduzir Requisitos)**
* **Diagnóstico:** Atender pequenos clientes ou defender soluções técnicas em entrevistas exige explicar o impacto prático do sistema, e não apenas a linguagem utilizada.
* **Ação concreta de treino:** Estruture o `README.md` de cada repositório no GitHub respondendo a três perguntas diretas: qual problema de negócio a ferramenta resolve, quais decisões de arquitetura foram tomadas para viabilizá-la e como qualquer pessoa pode testar a aplicação em produção.



---

Qual nicho ou tipo de sistema para pequenos negócios você planeja priorizar como primeiro projeto para validar esse ciclo de 90 dias?
