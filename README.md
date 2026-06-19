# 🚀 Sprint Master — Sistema de Gestão de Projetos de Pesquisa

MVP de aplicação web para gerenciamento de projetos e atividades de grupos de pesquisa.

---

## 👥 Equipe

| Nome                          | Papel        |
|-------------------------------|--------------|
| Elizabeth Fernandes Pires     | Scrum Master |
| Renan Dorio da Silva          | Product Owner|
| Klaus Marrer                  | Dev Backend  |
| William de Oliveira Santos    | Dev Frontend |
| Luca Vinicius Dourado Pessoa  | QA / Tester  |

---

## 🛠️ Stack Tecnológica

- **Backend:** Node.js + Express
- **Template Engine:** EJS
- **Banco de Dados:** SQLite (via `better-sqlite3`)
- **Frontend:** HTML/CSS puro + Bootstrap 5
- **Controle de versão:** Git + GitHub

---

## ⚙️ Como Rodar o Projeto

### Pré-requisitos

- Node.js >= 18.x instalado
- npm >= 9.x

### Instalação

```bash
# Clone o repositório
git clone https://github.com/williamoliveira-red/sprint-master.git
cd sprint-master

# Instale as dependências
npm install

# Inicie o servidor
npm start
```

A aplicação estará disponível em: **http://localhost:3000**

### Variáveis de ambiente (opcional)

Crie um arquivo `.env` na raiz:

```env
PORT=3000
DB_PATH=./database/sprint_master.db
```

---

## 📦 Funcionalidades Implementadas

- [x] Cadastro de projetos (nome, descrição, prazo)
- [x] Listagem de projetos
- [x] Cadastro de atividades vinculadas a um projeto (título, responsável, status)
- [x] Atualização de status das atividades (A Fazer / Em Andamento / Concluído)
- [x] Dashboard com % de conclusão por projeto

## 🚧 Não Implementado (Backlog Futuro)

- [ ] Edição de projetos existentes
- [ ] Exclusão de atividades
- [ ] Autenticação de usuário (login/senha)
- [ ] Notificações de prazo

---

## 📁 Estrutura de Arquivos

```
sprint-master/
├── app.js
├── package.json
├── database/
│   └── schema.sql
├── routes/
│   ├── projects.js
│   └── activities.js
├── views/
│   ├── index.ejs
│   ├── projects/
│   │   ├── list.ejs
│   │   ├── new.ejs
│   │   └── show.ejs
│   └── partials/
│       ├── header.ejs
│       └── footer.ejs
├── public/
│   └── css/
│       └── style.css
├── README.md
├── SPRINT_BACKLOG.md
├── DAILY_LOGS.md
└── RETROSPECTIVE.md
```

---

## 📄 Documentação da Sprint

- [`SPRINT_BACKLOG.md`](./SPRINT_BACKLOG.md) — Histórias de usuário e tarefas da sprint
- [`DAILY_LOGS.md`](./DAILY_LOGS.md) — Registro das dailies diárias
- [`RETROSPECTIVE.md`](./RETROSPECTIVE.md) — Retrospectiva Start/Stop/Continue
