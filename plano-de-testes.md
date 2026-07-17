# Plano de testes

## 1. Introdução e Objetivo
Este plano de teste tem como objetivo documentar a estratégia, o escopo e os critérios utilizados para testar as funcionalidades críticas do SauceDemo, um site de demonstração que simula um e-commerce, usado como ambiente de prática para QA.

## 2. Escopo
**Dentro do escopo:** Login, carrinho e checkout — funcionalidades de alta prioridade, com casos de teste completos usando técnicas de design de teste.

**Fora do escopo:** Filtro, visualização de produto, logout, reset app state e all items — funcionalidades de média e baixa prioridade, mapeadas e analisadas na fase de risco, mas não testadas neste ciclo, por decisão de priorização baseada em risco.

## 3. Estratégia de Teste
Primeiro foi usada a técnica de partição de equivalência nas três funcionalidades — login, carrinho e checkout — para identificar os grupos que tinham o mesmo comportamento no sistema. No caso do login, foi aplicada também tabela de decisão para mapear as combinações entre usuário e senha. Com essas técnicas, os casos de teste foram planejados priorizando os cenários mais relevantes de cada funcionalidade.

## 4. Critérios de Entrada
- Casos de teste elaborados e revisados
- Ambiente de teste (SauceDemo) disponível e acessível

## 5. Critérios de Saída
- Todos os casos de teste de prioridade alta executados
- Taxa de aprovação acima de 90%
- Defeitos críticos e altos documentados e comunicados, mesmo que não corrigidos

## 6. Análise de Risco
[analise-e-estrategia-de-teste.md](https://github.com/lidi-danelon/portfolio-lidi/blob/main/analise-e-estrat%C3%A9gia-de-teste.md#an%C3%A1lise-e-estrat%C3%A9gia-de-teste)

## 7. Métricas
- **Taxa de aprovação:** 95,24% (20 de 21 [casos](https://app.notion.com/p/Casos-de-teste-portf-lio-GitHub-3977092cc8e980b881e5f3ac52180ee2?source=copy_link) aprovados)
- **Cobertura de funcionalidades:** 58% (7 de 12 [funcionalidades mapeadas](https://github.com/lidi-danelon/portfolio-lidi/blob/main/analise-e-estrat%C3%A9gia-de-teste.md#an%C3%A1lise-e-estrat%C3%A9gia-de-teste))
- **Defeitos encontrados:** 1 (ID 1 — checkout aceita carrinho vazio, severidade alta)
