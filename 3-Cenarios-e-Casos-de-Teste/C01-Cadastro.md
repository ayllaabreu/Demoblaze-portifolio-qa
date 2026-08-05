# Cenário 01 — Cadastro

**Descrição:** Esse módulo cobre os testes relacionados ao cadastro de novos 
usuários no DemoBlaze. Testei o fluxo esperado e também 
situações onde o usuário pode errar ou tentar burlar o sistema.

---

## C01-CT01 — Cadastro com dados válidos

| Campo | Detalhe |
|-------|---------|
| **ID** | C01-CT01 |
| **Descrição** | Cadastro realizado com username e senha válidos |
| **Pré-condições** | O username utilizado não pode estar cadastrado no sistema |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E clico em "Sign up" no menu |
| 3 | E preencho o campo "Username" com um nome único |
| 4 | E preencho o campo "Password" com uma senha |
| 5 | QUANDO clico no botão "Sign up" |
| 6 | ENTÃO devo ver uma mensagem de cadastro realizado com sucesso |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve exibir uma mensagem confirmando o cadastro |
| **Resultado esperado** | Mensagem de sucesso exibida após o clique em "Sign up" |
| **Resultado real** | Mensagem "Sign up successful." exibida com sucesso |
| **Evidência** | ![C01-CT01](6-Evidencias/C01-Cadastro/C01-CT01-cadastro-valido.png) |
| **Status** | ✅ Aprovado |

---

## C01-CT02 — Cadastro com username já existente

| Campo | Detalhe |
|-------|---------|
| **ID** | C01-CT02 |
| **Descrição** | Tentativa de cadastro com um username que já está em uso |
| **Pré-condições** | Já deve existir um usuário cadastrado com o username utilizado no teste |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que já existe um usuário cadastrado com o username "aylla_teste" |
| 2 | E estou na tela de cadastro |
| 3 | E preencho o campo "Username" com "aylla_teste" |
| 4 | E preencho o campo "Password" com qualquer senha |
| 5 | QUANDO clico no botão "Sign up" |
| 6 | ENTÃO devo ver uma mensagem informando que o usuário já existe |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema não deve permitir o cadastro e deve informar o motivo |
| **Resultado esperado** | Mensagem de erro informando que o username já está em uso |
| **Resultado real** | Mensagem "This user already exist." exibida corretamente |
| **Evidência** | ![C01-CT02](../../6-Evidencias/C01-Cadastro/C01-CT02-username-existente.png) |
| **Status** | ✅ Aprovado |

---

## C01-CT03 — Cadastro com campos vazios

| Campo | Detalhe |
|-------|---------|
| **ID** | C01-CT03 |
| **Descrição** | Tentativa de cadastro sem preencher nenhum campo |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que abri o formulário de cadastro |
| 2 | E deixei os campos "Username" e "Password" em branco |
| 3 | QUANDO clico no botão "Sign up" |
| 4 | ENTÃO o sistema deve me avisar que os campos são obrigatórios |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve bloquear o cadastro e exibir aviso de campo obrigatório |
| **Resultado esperado** | Alerta informando que os campos precisam ser preenchidos |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |
