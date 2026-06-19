# 📋 Sprint Backlog — Sprint Master

**Sprint:** Sprint 1  
**Período:** 15/06/2026 (Segunda) a 19/06/2026 (Sexta)  
**Equipe:** Elizabeth Fernandes Pires, Renan Dorio da Silva, Klaus Marrer, William de Oliveira Santos, Luca Vinicius Dourado Pessoa  

---

## 🧾 Histórias de Usuário

### US-01 — Cadastro de Projetos
> *"Como chefe do grupo, quero cadastrar um projeto com nome, descrição e prazo, para organizar os trabalhos do grupo."*

**Critérios de Aceitação:**
- Formulário com campos: Nome (obrigatório), Descrição (obrigatório), Prazo (data, obrigatório)
- Projeto aparece na listagem após o cadastro
- Validação: campos obrigatórios não podem ficar vazios

**Estimativa:** M (5 pontos)  
**Responsável:** Klaus Marrer (backend) + William de Oliveira Santos (frontend)  
**Status:** ✅ Concluído

---

### US-02 — Gerenciamento de Atividades
> *"Como chefe do grupo, quero adicionar atividades a um projeto, informando título, responsável e status (A Fazer / Em Andamento / Concluído), para distribuir e acompanhar o trabalho."*

**Critérios de Aceitação:**
- Formulário de nova atividade vinculado a um projeto
- Campo de status com as três opções
- Possibilidade de alterar o status da atividade após criação
- Listagem de atividades na página do projeto

**Estimativa:** L (8 pontos)  
**Responsável:** Klaus Marrer + William de Oliveira Santos  
**Status:** ✅ Concluído (edição de status OK; exclusão ficou fora do escopo)

---

### US-03 — Dashboard de Acompanhamento
> *"Como chefe do grupo, quero ver um dashboard com todos os projetos e a porcentagem de conclusão de cada um, para ter uma visão geral do andamento do grupo."*

**Critérios de Aceitação:**
- Página inicial exibe todos os projetos cadastrados
- Cada card de projeto mostra: nome, prazo e % de atividades concluídas
- Barra de progresso visual para cada projeto

**Estimativa:** M (5 pontos)  
**Responsável:** William de Oliveira Santos (frontend) + Klaus Marrer (lógica de cálculo)  
**Status:** ✅ Concluído

---

## 🗂️ Tarefas Técnicas (Tasks)

| ID   | Tarefa                                                     | Responsável                   | Estimativa | Status       |
|------|------------------------------------------------------------|-------------------------------|------------|--------------|
| T-01 | Configurar repositório GitHub e branches                   | Elizabeth Fernandes Pires     | S (1pt)    | ✅ Concluído |
| T-02 | Setup Node.js + Express + EJS                              | Klaus Marrer                  | S (1pt)    | ✅ Concluído |
| T-03 | Criar schema do banco SQLite (tabelas projects/activities) | Klaus Marrer                  | S (2pt)    | ✅ Concluído |
| T-04 | Endpoint POST /projects (criar projeto)                    | Klaus Marrer                  | S (2pt)    | ✅ Concluído |
| T-05 | Endpoint GET /projects (listar projetos)                   | Klaus Marrer                  | S (1pt)    | ✅ Concluído |
| T-06 | Endpoint POST /activities (criar atividade)                | Klaus Marrer                  | S (2pt)    | ✅ Concluído |
| T-07 | Endpoint PATCH /activities/:id/status                      | Klaus Marrer                  | M (3pt)    | ✅ Concluído |
| T-08 | View EJS: formulário de novo projeto                       | William de Oliveira Santos    | S (2pt)    | ✅ Concluído |
| T-09 | View EJS: listagem de projetos (dashboard)                 | William de Oliveira Santos    | M (3pt)    | ✅ Concluído |
| T-10 | View EJS: página do projeto com atividades                 | William de Oliveira Santos    | M (3pt)    | ✅ Concluído |
| T-11 | Barra de progresso com % calculado no backend              | William de Oliveira Santos    | S (2pt)    | ✅ Concluído |
| T-12 | Estilização com Bootstrap 5                                | William de Oliveira Santos    | S (2pt)    | ✅ Concluído |
| T-13 | Testes manuais: CRUD de projetos                           | Luca Vinicius Dourado Pessoa  | M (3pt)    | ✅ Concluído |
| T-14 | Testes manuais: CRUD de atividades + mudança status        | Luca Vinicius Dourado Pessoa  | M (3pt)    | ✅ Concluído |
| T-15 | Testes manuais: dashboard e % de conclusão                 | Luca Vinicius Dourado Pessoa  | S (2pt)    | ✅ Concluído |
| T-16 | Registro das dailies no DAILY_LOGS.md                      | Elizabeth Fernandes Pires     | S (1pt)    | ✅ Concluído |
| T-17 | Preparar slides da Sprint Review                           | Renan Dorio da Silva          | S (2pt)    | ✅ Concluído |
| T-18 | Escrever RETROSPECTIVE.md                                  | Elizabeth Fernandes Pires     | S (1pt)    | ✅ Concluído |
| T-19 | Finalizar README.md                                        | Elizabeth Fernandes Pires     | S (1pt)    | ✅ Concluído |
| T-20 | Edição de projetos existentes                              | —                             | M (3pt)    | ❌ Não feito |
| T-21 | Exclusão de atividades                                     | —                             | S (2pt)    | ❌ Não feito |

---

## 📊 Resumo da Sprint

| Métrica                    | Valor    |
|----------------------------|----------|
| Total de pontos planejados | 43 pts   |
| Pontos entregues           | 38 pts   |
| Velocidade da equipe       | 88%      |
| Histórias 100% aceitas     | 3 de 3   |
| Tarefas concluídas         | 19 de 21 |

---

## 📌 Definition of Done

Uma história é considerada **pronta** quando:
1. O código está no branch `main` via Pull Request revisado
2. A funcionalidade passa nos testes manuais da QA (Luca)
3. O Product Owner (Renan) validou contra os critérios de aceitação
4. Não há bugs críticos abertos relacionados à história
