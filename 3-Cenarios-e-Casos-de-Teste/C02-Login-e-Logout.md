# Cenário 02 - Login e Logout

**Descrição:** Esse módulo cobre os testes de autenticação 
do DemoBlaze. Validei o login com diferentes situações — 
credenciais corretas, senha errada, usuário inexistente e 
campos vazios — e também o fluxo de logout.

---

## C02-CT01 - Login com credenciais válidas

| Campo | Detalhe |
|-------|---------|
| **ID** | C02-CT01 |
| **Descrição** | Login realizado com username e senha corretos |
| **Pré-condições** | Usuário deve estar cadastrado no sistema |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que tenho uma conta cadastrada no DemoBlaze |
| 2 | E estou na página inicial do DemoBlaze |
| 3 | E clico em "Log in" no menu |
| 4 | E preencho o campo "Username" com meu username correto |
| 5 | E preencho o campo "Password" com minha senha correta |
| 6 | QUANDO clico no botão "Log in" |
| 7 | ENTÃO meu nome deve aparecer no menu de navegação |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve autenticar o usuário e exibir seu nome no menu |
| **Resultado esperado** | Usuário logado e nome visível no menu de navegação |
| **Resultado real** | Usuário logado com sucesso. Mensagem "Welcome aylla_teste" exibida no menu de navegação |
| **Evidência** | [C02-CT01-login-valido.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C02-Login-e-Logout/C02-CT01-login-valido.png) |
| **Status** | ✅ Aprovado |

---

## C02-CT02 - Login com senha incorreta

| Campo | Detalhe |
|-------|---------|
| **ID** | C02-CT02 |
| **Descrição** | Tentativa de login com username correto e senha errada |
| **Pré-condições** | Usuário deve estar cadastrado no sistema |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que tenho uma conta cadastrada no DemoBlaze |
| 2 | E estou na página inicial do DemoBlaze |
| 3 | E clico em "Log in" no menu |
| 4 | E preencho o campo "Username" com o username "aylla_teste" |
| 5 | E preencho o campo "Password" com uma senha errada |
| 6 | QUANDO clico no botão "Log in" |
| 7 | ENTÃO devo ver uma mensagem de erro de credenciais inválidas |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema não deve autenticar e deve informar que as credenciais estão erradas |
| **Resultado esperado** | Mensagem de erro exibida e usuário permanece na tela de login |
| **Resultado real** | Mensagem de erro "Wrong password." exibida com sucesso |
| **Evidência** | [C02-CT02-senha-incorreta.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C02-Login-e-Logout/C02-CT02-senha-incorreta.png) |
| **Status** | ✅ Aprovado |

---

## C02-CT03 - Login com usuário não cadastrado

| Campo | Detalhe |
|-------|---------|
| **ID** | C02-CT03 |
| **Descrição** | Tentativa de login com username que não existe no sistema |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E clico em "Log in" no menu |
| 3 | E preencho o campo "Username" com "xyzusuario999teste" |
| 4 | E preencho o campo "Password" com "senha123" |
| 5 | QUANDO clico no botão "Log in" |
| 6 | ENTÃO devo ver uma mensagem de erro informando que o usuário não foi encontrado |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema não deve autenticar e deve informar que o usuário não foi encontrado |
| **Resultado esperado** | Mensagem de erro exibida informando credenciais inválidas |
| **Resultado real** | Mensagem de erro "User does not exist." exibida com sucesso e usuário permanece na tela de login |
| **Evidência** | [C02-CT03-usuario-inexistente.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C02-Login-e-Logout/C02-CT03-usuario-inexistente.png) |
| **Status** | ✅ Aprovado |

---

## C02-CT04 - Login com campos vazios

| Campo | Detalhe |
|-------|---------|
| **ID** | C02-CT04 |
| **Descrição** | Tentativa de login sem preencher nenhum campo |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Média |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E clico em "Log in" no menu |
| 3 | E deixei os campos "Username" e "Password" em branco |
| 4 | QUANDO clico no botão "Log in" |
| 5 | ENTÃO o sistema deve me avisar que os campos são obrigatórios |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema não deve autenticar e deve informar que as credenciais estão erradas |
| **Resultado esperado** | Mensagem de erro exibida e usuário permanece na tela de login |
| **Resultado real** | Mensagem de erro "Please fill out Username and Password" exibida com sucesso e usuário permanece na tela de login |
| **Evidência** | [C02-CT04-campos-vazios.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C02-Login-e-Logout/C02-CT04-campos-vazios.png) |
| **Status** | ✅ Aprovado |

---

## C02-CT05 - Logout

| Campo | Detalhe |
|-------|---------|
| **ID** | C02-CT05 |
| **Descrição** | Usuário encerra a sessão pelo menu de navegação |
| **Pré-condições** | Usuário deve estar logado no sistema |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou logada no DemoBlaze |
| 2 | E meu nome aparece no menu de navegação |
| 3 | QUANDO clico em "Log out" no menu |
| 4 | ENTÃO meu nome deve desaparecer do menu |
| 5 | E as opções "Sign up" e "Log in" devem voltar a aparecer |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve encerrar a sessão e retornar ao estado de usuário deslogado |
| **Resultado esperado** | Menu exibe "Sign up" e "Log in" após o logout |
| **Resultado real** | Logout realizado com sucesso. Menu voltou a exibir "Log in" e "Sign up" |
| **Evidência** | [Antes](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C02-Login-e-Logout/C02-CT05-logout-antes.png) / [Depois](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C02-Login-e-Logout/C02-CT05-logout-depois.png) |
| **Status** | ✅ Aprovado |
