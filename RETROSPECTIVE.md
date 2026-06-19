# 🔄 Sprint Retrospective — Sprint 1

**Data:** 19/06/2026 (Sexta-feira, após a Review)  
**Facilitador:** Elizabeth Fernandes Pires (Scrum Master)  
**Participantes:** Elizabeth Fernandes Pires, Renan Dorio da Silva, Klaus Marrer, William de Oliveira Santos, Luca Vinicius Dourado Pessoa  
**Técnica utilizada:** Start / Stop / Continue  
**Duração:** ~25 minutos

---

## ✅ CONTINUE — O que está dando certo e devemos manter

1. **Comunicação pelo Discord**  
   O grupo criou canais separados por tema (`#geral`, `#bugs`, `#código`, `#daily`). Isso manteve as conversas organizadas e evitou ruído. Todo mundo leu as mensagens no tempo certo.

2. **Divisão clara de papéis desde o início**  
   Saber desde o dia 1 quem era Dev, QA, PO e SM eliminou disputas e duplicação de trabalho. O Luca, por exemplo, ficou focado em testar — não precisou adivinhar se era responsabilidade dele ou do Dev abrir issues.

3. **Pull Requests com revisão antes do merge**  
   Mesmo sendo um projeto pequeno, a prática de abrir PR e pelo menos uma pessoa revisar antes de mergear evitou três possíveis conflitos de código que identificamos depois.

4. **Dailies curtas e objetivas**  
   Nenhuma daily passou de 15 minutos. O formato das três perguntas funcionou bem: todo mundo sabia o que falar e não havia espaço para virar reunião de status longa.

5. **QA entrando cedo no processo**  
   O Luca começou a montar os casos de teste já no Dia 1, antes mesmo de ter código para testar. Isso acelerou muito a validação quando os endpoints ficaram prontos.

---

## 🛑 STOP — O que devemos parar de fazer

1. **Commitar diretamente na branch `main`**  
   No Dia 1, antes de Elizabeth configurar a proteção da branch, dois commits foram para o `main` diretamente. Precisamos garantir que isso nunca mais aconteça — e ativar a proteção de branch no GitHub desde o início.

2. **Resolver bugs "no bate-papo" sem abrir issue**  
   Alguns problemas menores foram corrigidos sem registro. Isso dificulta rastrear o histórico de decisões e pode fazer o mesmo bug voltar sem que a equipe saiba que já aconteceu antes.

3. **Deixar a integração frontend/backend para o final**  
   William e Klaus trabalharam em paralelo nos primeiros dias sem integrar. Quando foi integrar no Dia 4, surgiram pequenas incompatibilidades (nome de campos no JSON). Se tivéssemos combinado um contrato de API antes, economizaríamos tempo.

4. **Reuniões sem pauta prévia**  
   A Planning durou um pouco mais que o esperado porque entramos sem uma ordem de discussão definida. Da próxima vez, o PO deve chegar com a pauta escrita antes.

---

## 🚀 START — O que devemos começar a fazer

1. **Usar branches por feature (ex: `feature/cadastro-projeto`)**  
   Trabalhamos majoritariamente em `develop` sem sub-branches. Na próxima sprint, cada tarefa deve ter sua própria branch, facilitando revisão de código e permitindo trabalhar em paralelo sem conflitos.

2. **Definir um contrato de API antes de codificar (API-first)**  
   Antes de Klaus e William começarem a codar separado, devemos sentar juntos e anotar os endpoints: rota, método, corpo esperado e resposta. Um arquivo `api-contract.md` simples já resolve.

3. **Fazer ao menos uma sessão de pair programming por sprint**  
   Klaus e William nunca se sentaram juntos para codar. Uma sessão de pair teria acelerado a integração e disseminado conhecimento — ambos entenderiam tanto o backend quanto o frontend.

4. **Gravar a Review em vídeo**  
   Não gravamos a demonstração. Teria sido útil para portfólio, para consulta futura e para membros que porventura faltassem. Na próxima, gravamos via Google Meet.

5. **Estimar com mais base (usar referência histórica)**  
   Algumas tarefas foram estimadas em S e levaram muito mais tempo. Com uma sprint no histórico agora, podemos calibrar melhor as estimativas na próxima Planning.

---

## 🎯 Ações de Melhoria (pelo menos 2 para a próxima Sprint)

| # | Ação | Responsável | Prazo |
|---|------|-------------|-------|
| 1 | Ativar proteção de branch no GitHub (impedir push direto para `main` e `develop`) | Elizabeth Fernandes Pires | Dia 1 da próxima Sprint |
| 2 | Criar arquivo `api-contract.md` na Planning antes de começar qualquer desenvolvimento | Renan Dorio da Silva + Klaus + William | Dia 1 da próxima Sprint |
| 3 | Criar uma branch por feature a partir de `develop` (padrão acordado: `feature/nome-curto`) | Todos os devs | A partir da próxima Sprint |
| 4 | Gravar a Sprint Review pelo Google Meet | Elizabeth Fernandes Pires (organizar gravação) | Próxima Review |

---

## 💬 Sentimento Geral da Equipe

> *Escala de 1 a 5 — perguntado anonimamente pelo facilitador no Discord antes da retro.*

| Membro | Satisfação com a Sprint | Comentário (opcional) |
|--------|-------------------------|-----------------------|
| Elizabeth Fernandes Pires | ⭐⭐⭐⭐ (4/5) | "Gostei da organização. Próxima, quero ver mais commits descritivos." |
| Renan Dorio da Silva | ⭐⭐⭐⭐ (4/5) | "Produto saiu funcional. Faltou edição de projetos, mas entendemos o porquê." |
| Klaus Marrer | ⭐⭐⭐⭐⭐ (5/5) | "Aprendi muito sobre SQLite. O ambiente de testes do Luca me ajudou muito." |
| William de Oliveira Santos | ⭐⭐⭐ (3/5) | "Queria ter integrado antes. Aprendi a lição sobre API-first na prática." |
| Luca Vinicius Dourado Pessoa | ⭐⭐⭐⭐ (4/5) | "Gostei de ter entrado cedo. A questão do reload da % ficou como aprendizado." |

**Média:** 4.0 / 5.0

---

*Documento redigido por Elizabeth Fernandes Pires em 19/06/2026.*
