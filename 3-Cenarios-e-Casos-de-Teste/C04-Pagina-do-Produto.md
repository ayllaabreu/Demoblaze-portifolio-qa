# Cenário 04 - Página do Produto

**Descrição:** Esse módulo valida o comportamento da página 
de detalhes de um produto. Verifiquei se as informações 
aparecem corretamente e se os diferentes caminhos para 
acessar a página funcionam como esperado.

---

## C04-CT01 - Acessar a página do produto pelo nome

| Campo | Detalhe |
|-------|---------|
| **ID** | C04-CT01 |
| **Descrição** | Verificar se clicar no nome do produto abre a página de detalhes |
| **Pré-condições** | Pelo menos um produto deve estar visível na página inicial |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E consigo ver a listagem de produtos |
| 3 | QUANDO clico no nome de um produto |
| 4 | ENTÃO devo ser redirecionada para a página de detalhes desse produto |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | A página de detalhes do produto clicado deve ser aberta corretamente |
| **Resultado esperado** | Redirecionamento para a página de detalhes do produto |
| **Resultado real** | Redirecionamento para a página de detalhes do Samsung Galaxy S6 realizado com sucesso |
| **Evidência** | [C04-CT01-acesso-pelo-nome.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C04-Pagina-do-Produto/C04-CT01-acesso-pelo-nome.png) |
| **Status** | ✅ Aprovado |

---

## C04-CT02 - Acessar a página do produto pela foto

| Campo | Detalhe |
|-------|---------|
| **ID** | C04-CT02 |
| **Descrição** | Verificar se clicar na foto do produto também abre a página de detalhes |
| **Pré-condições** | Pelo menos um produto deve estar visível na página inicial |
| **Prioridade** | Média |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E consigo ver a listagem de produtos com suas fotos |
| 3 | QUANDO clico na foto de um produto |
| 4 | ENTÃO devo ser redirecionada para a página de detalhes desse produto |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | A página de detalhes do produto clicado deve ser aberta corretamente |
| **Resultado esperado** | Redirecionamento para a página de detalhes do produto |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |

---

## C04-CT03 - Verificar informações exibidas na página do produto

| Campo | Detalhe |
|-------|---------|
| **ID** | C04-CT03 |
| **Descrição** | Verificar se todas as informações do produto aparecem corretamente na página de detalhes |
| **Pré-condições** | Estar na página de detalhes de um produto |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que acessei a página de detalhes de um produto |
| 2 | ENTÃO devo ver o nome do produto |
| 3 | E devo ver a foto do produto |
| 4 | E devo ver a descrição do produto |
| 5 | E devo ver o preço do produto |
| 6 | E devo ver o botão "Add to cart" |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | Nome, foto, descrição, preço e botão "Add to cart" devem estar visíveis e corretos |
| **Resultado esperado** | Todas as informações do produto exibidas corretamente na página |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |

---

## C04-CT04 - Voltar ao catálogo a partir da página do produto

| Campo | Detalhe |
|-------|---------|
| **ID** | C04-CT04 |
| **Descrição** | Verificar se é possível voltar ao catálogo sem perder a listagem de produtos |
| **Pré-condições** | Estar na página de detalhes de um produto |
**Prioridade** | Baixa |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página de detalhes de um produto |
| 2 | QUANDO clico no logo do DemoBlaze ou em "Home" no menu |
| 3 | ENTÃO devo ser redirecionada para a página inicial |
| 4 | E a listagem de produtos deve aparecer normalmente |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | A navegação de volta ao catálogo deve funcionar sem erros |
| **Resultado esperado** | Página inicial carregada corretamente com todos os produtos visíveis |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |
