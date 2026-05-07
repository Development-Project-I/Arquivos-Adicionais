# 📄 Status Report – Sprint 2

## 👥 Equipe

* **Nome do projeto:** GastroPlan
* **Integrantes:** Cleber Moraes, Gustavo Müller, Herian Souza, Lucas Capoani e Roberto Souza
* **Scrum Master da Sprint:** Cleber Moraes
* **Product Owner:** Lucas Capoani

---

## 📅 Informações da Sprint

* **Número da Sprint:** 2
* **Período:** 23/04 – 07/05
* **Objetivo da Sprint:**

> Implementar a base do backend com NestJS e TypeORM, configurar o banco de dados PostgreSQL, criar os módulos de Inventário e Usuários com CRUD completo e validações, e avançar no front-end com o desenvolvimento da tela de login.

---

## 📌 1. Resumo Executivo

Nesta sprint, a equipe focou na implementação do backend da aplicação utilizando NestJS com TypeORM e PostgreSQL. Foram criados os módulos de Inventário (com CRUD completo e sistema de alertas de status) e Usuários (com cadastro seguro via hash de senha e validações). No front-end, houve avanço geral e a tela de login foi iniciada, estando em andamento.

* **A sprint foi:**

  * ( ) Concluída com sucesso
  * (X) Parcialmente concluída
  * ( ) Não concluída

* **Principais entregas:**

  * Módulo de Inventário com CRUD e alertas de status
  * Módulo de Usuários com cadastro seguro (bcrypt)
  * DTOs com validação via class-validator
  * Testes de usabilidade e validação dos endpoints via Postman
  * Avanço no front-end

* **Principais dificuldades:**

  * Configuração e integração do TypeORM com PostgreSQL
  * Definição da estrutura de entidades e relacionamentos

---

## ✅ 2. Itens Planejados vs Entregues

**Status possíveis (utilizar apenas estes):**

* 🟢 Concluído
* 🟡 Em andamento
* 🔴 Não iniciado
* ⚫ Bloqueado

| User Story / Tarefa                                          | Responsável | Story Points | Status | Observações                            |
| ------------------------------------------------------------ | ----------- | ------------ | ------ | -------------------------------------- |
| US01 – Estrutura base do backend (NestJS)                    | Roberto     | 3            | 🟢     |                                        |
| US02 – Configuração do banco de dados (TypeORM + PostgreSQL) | Roberto     | 3            | 🟢     |                                        |
| US03 – Módulo de Inventário – CRUD completo                  | Lucas       | 5            | 🟢     |                                        |
| US04 – Sistema de alertas de status no inventário            | Lucas       | 2            | 🟢     | Esgotado, Vencido e Estoque Baixo      |
| US05 – Módulo de Usuários – cadastro com hash de senha       | Lucas       | 3            | 🟢     | Senhas protegidas com bcrypt           |
| US06 – DTOs com validação (class-validator)                  | Lucas       | 2            | 🟢     | Validações em Inventário e Usuários    |
| US07 – Tela de login (front-end)                             | Gustavo     | 3            | 🟡     | Em andamento                           |
| US08 – Avanço geral do front-end                             | Gustavo     | 3            | 🟡     | Em andamento                           |
| US09 – Testes de usabilidade e validação de endpoints (QA)   | Herian      | 3            | 🟢     | Testes manuais via Postman e testes de usabilidade |

---

## 🚀 3. Entregas da Sprint

### Funcionalidades implementadas

* Módulo de Inventário com endpoints REST (POST, GET, GET por ID, PATCH, DELETE)
* Alertas automáticos de status dos itens (Esgotado, Vencido, Estoque Baixo)
* Módulo de Usuários com endpoint de cadastro (`POST /users/register`)
* Hash seguro de senhas com bcrypt
* Validação de duplicidade de e-mail e matrícula
* DTOs com validações robustas via class-validator

### Evidências (obrigatório)

* **Link do repositório:** https://github.com/Development-Project-I
* **Link do quadro Kanban:** https://projeto-de-desenvolvimento1.atlassian.net/jira/software/projects/PDD1/boards/2
* **Link do deploy (se houver):** 

---

## 🧪 4. Qualidade e Testes

* **Tipos de testes realizados:** Testes manuais via Postman nos endpoints do backend e testes de usabilidade

* **Responsável pelos testes (QA):** Herian Souza

* **Cobertura (se aplicável):** Não aplicável

* **Bugs encontrados:** 0

* **Bugs corrigidos:** 0

---

## 🔧 5. Processo e Ferramentas

* **Controle de versão utilizado:** Git + GitHub
* **Estratégia de branch:** feature branches + main
* **Uso de CI/CD:** Não utilizado nesta sprint
* **Ferramentas utilizadas:** NestJS, TypeORM, PostgreSQL, bcrypt, class-validator, Typescript, React, Figma, Jira

---

## ⚠️ 6. Impedimentos

Sem impedimentos até o momento

---

## 🔄 7. Retrospectiva da Sprint

### 👍 O que funcionou bem

* Boa divisão entre tarefas de backend e front-end
* Implementação do backend seguiu boas práticas (DTOs, validações, hash de senha)
* Comunicação eficiente no grupo

### 👎 O que pode melhorar

* Integração entre front-end e backend ainda não iniciada
* Tela de login não foi finalizada dentro da sprint
* Melhor sincronização entre o time de front e back

### 🔁 Ações para próxima sprint

* Finalizar a tela de login
* Iniciar a integração front-end ↔ backend
* Implementar autenticação JWT
* Expandir o front-end com as páginas de inventário

---

## 📊 8. Métricas da Sprint

* **Story Points planejados:** 27

* **Story Points concluídos:** 21

* **Velocidade da equipe:**

> 21 story points concluídos de 27 planejados (78% de entrega)

* **% Entrega:**

> 78%

* **Nº de tarefas concluídas:** 7
* **Nº de tarefas não concluídas:** 2
* **Nº de commits:** 
* **Nº de PRs:** 

---

## 🎯 9. Planejamento Inicial da Próxima Sprint

* **Principais objetivos:**

  * Finalizar a tela de login
  * Implementar autenticação JWT no backend
  * Iniciar integração front-end com a API
  * Desenvolver a tela de inventário no front-end

* **Riscos identificados:**

  * Complexidade da integração autenticação + front-end
  * Prazo curto para implementar JWT e tela de login ao mesmo tempo
