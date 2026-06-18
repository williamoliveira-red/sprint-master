# 📅 Daily Logs — Sprint 1

**Projeto:** Sprint Master  
**Responsável pelos registros:** Elizabeth Fernandes Pires (Scrum Master)  
**Formato:** Presencial + Discord (nos dias remotos)  
**Horário padrão das dailies:** 09h00 — 09h15

---

## Daily #1 — Segunda-feira, 15/06/2026

**Tipo:** Pós-Planning (realizada ao final do dia 1)  
**Participantes:** Elizabeth Fernandes Pires ✅ | Renan Dorio da Silva ✅ | Klaus Marrer ✅ | William de Oliveira Santos ✅ | Luca Vinicius Dourado Pessoa ✅  
**Impedimentos reportados:** Nenhum

### Registro

| Membro | O que fiz hoje? | O que farei amanhã? | Impedimentos? |
|--------|-----------------|---------------------|---------------|
| **Elizabeth** | Criei o repositório no GitHub, configurei a branch `develop` e adicionei o time como colaborador. Documentei a estrutura de pastas. | Monitorar o progresso do setup e registrar daily. | Nenhum. |
| **Renan** | Conduzi a Planning como PO: apresentei as 3 histórias de usuário, refinamos os critérios de aceitação com a equipe. | Validar o backlog criado e tirar dúvidas da equipe sobre requisitos. | Nenhum. |
| **Klaus** | Fiz o setup do Node.js + Express + EJS, criei o `package.json` e o arquivo `schema.sql` com as tabelas `projects` e `activities`. | Implementar os endpoints `POST /projects` e `GET /projects`. | Precisei pesquisar a lib `better-sqlite3` — resolvido. |
| **William** | Escolhi o Bootstrap 5 como framework de estilo, criei a estrutura base das views EJS (header/footer parciais). | Montar o formulário de novo projeto. | Nenhum. |
| **Luca** | Li as histórias de usuário e montei um checklist de testes manuais para cada critério de aceitação. | Aguardar o primeiro endpoint ficar pronto para já começar a testar. | Nenhum. |

---

## Daily #2 — Terça-feira, 16/06/2026

**Tipo:** Presencial  
**Participantes:** Elizabeth Fernandes Pires ✅ | Renan Dorio da Silva ✅ | Klaus Marrer ✅ | William de Oliveira Santos ✅ | Luca Vinicius Dourado Pessoa ✅  
**Impedimentos reportados:** 1 (resolvido na hora)

### Registro

| Membro | O que fiz ontem? | O que farei hoje? | Impedimentos? |
|--------|------------------|-------------------|---------------|
| **Elizabeth** | Acompanhei o repositório, revisei os commits do dia 1. | Garantir que todos façam PRs para `develop` e não diretamente para `main`. | Nenhum. |
| **Renan** | Estive disponível para responder dúvidas de requisito. Confirmei que "prazo" é uma data simples (sem hora). | Preparar rascunho dos slides da Review. | Nenhum. |
| **Klaus** | Implementei `POST /projects` e `GET /projects` com validação básica. Banco SQLite criado e funcionando. | Começar os endpoints de atividades: `POST /activities` e `GET /activities/:projectId`. | Dúvida sobre relacionamento do banco — Renan esclareceu que cada atividade pertence a um único projeto. ✅ |
| **William** | Formulário de novo projeto pronto no EJS, conectado ao endpoint do Klaus. | Montar a view de listagem de projetos (dashboard). | Nenhum. |
| **Luca** | Testei o endpoint `POST /projects` com dados válidos e inválidos (campo vazio). Encontrei bug: campos em branco não retornavam erro. | Reportar o bug ao Klaus e continuar testes da listagem. | Bug reportado como issue #3 no GitHub. |

**🐛 Bug registrado:** Issue #3 — Validação ausente em campos obrigatórios de projeto. Atribuído ao Klaus.

---

## Daily #3 — Quarta-feira, 17/06/2026

**Tipo:** Presencial  
**Participantes:** Elizabeth Fernandes Pires ✅ | Renan Dorio da Silva ✅ | Klaus Marrer ✅ | William de Oliveira Santos ✅ | Luca Vinicius Dourado Pessoa ✅  
**Impedimentos reportados:** Nenhum

### Registro

| Membro | O que fiz ontem? | O que farei hoje? | Impedimentos? |
|--------|------------------|-------------------|---------------|
| **Elizabeth** | Revisei os commits e fiz merge do PR do Klaus após revisão. | Atualizar o SPRINT_BACKLOG.md com status das tarefas. | Nenhum. |
| **Renan** | Validei o formulário de criação de projeto no ambiente local. | Rever os critérios de aceitação da US-02 (atividades). | Nenhum. |
| **Klaus** | Corrigi a validação (Issue #3 fechada ✅). Implementei `POST /activities`. | Implementar `PATCH /activities/:id/status` e lógica de % no GET /projects. | Nenhum. |
| **William** | Dashboard (listagem de projetos) pronto, exibindo nome e prazo de cada projeto. | Adicionar barra de progresso ao card do projeto (aguardando % do Klaus). | Dependência do endpoint do Klaus — combinado de ele entregar hoje. |
| **Luca** | Testei a criação de atividades. Encontrei problema: não havia feedback visual ao salvar. | Levantar requisitos visuais mínimos (mensagem de sucesso/erro) e discutir com William. | Nenhum. |