# Plano de reformulação e implantação

## Escopo e referência temporal

Este plano cobre os desafios recebidos até 25 de agosto de 2026 no marcador de e-mail `10 7DaysOfCode`: dias 1 a 4 do desafio de Prompt Engineering.

## Diagnóstico da estrutura atual

- Os dias 1 e 2 estão documentados em `desafios/`, com contexto, prompts e resultados.
- O Dia 3 possui um prompt em `prompts/` e o enunciado bruto em `resultados/dia03/`, mas não possui resumo conceitual nem registro diário consolidado em `desafios/`.
- O Dia 4 ainda não possui conceito, desafio, prompt ou estrutura de resultado.
- Os templates existentes cobrem registro diário, comparação e execução, mas não separam claramente plano de teste, critérios objetivos e resultado a ser preenchido.
- Não existem diretórios de testes dentro de cada dia de resultado.
- O README não reflete o progresso parcial do Dia 3 nem o desafio recebido no Dia 4.

## Reformulação proposta

1. Preservar a organização principal (`conceitos`, `contexto`, `desafios`, `prompts`, `resultados` e `templates`).
2. Consolidar cada técnica em `conceitos/` e cada atividade em `desafios/`.
3. Manter em `prompts/` apenas prompts prontos para serem copiados e executados.
4. Criar `resultados/diaXX/testes/` para definir os testes de cada desafio sem executá-los.
5. Manter os arquivos de resultados como esqueletos, para preenchimento manual após a execução dos prompts.
6. Usar critérios verificáveis e evitar depender de raciocínio interno do modelo; no Dia 4, solicitar análise resumida e fatores observáveis.

## Implantação

### Fase 1 — Normalização dos dias existentes

- Criar a documentação consolidada do Dia 3.
- Criar o resumo de Few-Shot Prompting.
- Ajustar o prompt do Dia 3 apenas quando necessário para consistência estrutural.
- Criar os diretórios e planos de teste dos dias 1, 2 e 3.

### Fase 2 — Implementação do desafio do dia presente

- Criar o resumo de Chain of Thought do Dia 4.
- Criar o registro do desafio do Dia 4 com o dilema derivado do plano do Dia 3.
- Criar um prompt completo do Dia 4, reutilizando persona, perfil base e plano semanal.
- Criar `resultados/dia04/testes/` e os esqueletos de resultado.

### Fase 3 — Templates e navegação

- Criar template de plano de teste com objetivo, entradas, procedimento manual, critérios e campos de evidência.
- Criar template de resultado separado do plano de teste.
- Atualizar o README para refletir o progresso até o Dia 4 e explicar a estrutura de testes.

## Critérios de aceite

- Todos os desafios recebidos até a data presente têm conceito, desafio e prompt rastreáveis.
- Cada dia de 1 a 4 possui um diretório `testes/` dentro de `resultados/diaXX/`.
- Nenhum teste é executado e nenhuma resposta de IA é inventada.
- Os arquivos de resultado permanecem vazios ou com campos explícitos para preenchimento.
- Links relativos e nomes de arquivos seguem o padrão já adotado no repositório.
- O conteúdo existente do usuário é preservado; alterações são aditivas ou correções pontuais justificadas.

## Ordem de execução

1. Criar este plano.
2. Criar os templates.
3. Completar e normalizar o Dia 3.
4. Implementar a estrutura do Dia 4.
5. Criar planos e esqueletos de teste dos dias 1 a 4.
6. Atualizar o README.
7. Verificar somente estrutura, links e diferenças do Git, sem executar testes dos desafios.
