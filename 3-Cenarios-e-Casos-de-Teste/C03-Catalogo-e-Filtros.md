# Cenário 03 — Catálogo e Filtros

**Descrição:** Esse módulo valida a exibição dos produtos 
na página inicial e o funcionamento dos filtros por categoria. 
Verifiquei se os produtos aparecem corretamente e se cada 
filtro realmente exibe apenas os itens da categoria selecionada.

---

## C03-CT01 — Visualizar produtos na página inicial

| Campo | Detalhe |
|-------|---------|
| **ID** | C03-CT01 |
| **Descrição** | Verificar se os produtos são exibidos corretamente ao acessar o site |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que acesso o DemoBlaze pelo navegador |
| 2 | QUANDO a página inicial termina de carregar |
| 3 | ENTÃO devo ver uma lista de produtos |
| 4 | E cada produto deve exibir nome, foto e preço |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | Os produtos devem ser exibidos com nome, foto e preço visíveis |
| **Resultado esperado** | Lista de produtos carregada corretamente na página inicial |
| **Resultado real** | Produtos exibidos corretamente com nome, foto e preço na página inicia) |
| **Evidência** | [C03-CT01-produtos-pagina-inicial.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C03-Catalogo-e-Filtros/C03-CT01-produtos-pagina-inicial.png) |
| **Status** | ✅ Aprovado |

---

## C03-CT02 — Filtrar produtos por Phones

| Campo | Detalhe |
|-------|---------|
| **ID** | C03-CT02 |
| **Descrição** | Verificar se o filtro de categoria Phones exibe apenas celulares |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E consigo ver todos os produtos listados |
| 3 | QUANDO clico na categoria "Phones" no menu lateral |
| 4 | ENTÃO a lista deve ser atualizada |
| 5 | E devo ver apenas produtos da categoria Phones |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | Apenas produtos da categoria Phones devem aparecer após o filtro |
| **Resultado esperado** | Lista atualizada exibindo somente celulares |
| **Resultado real** | Filtro aplicado corretamente, exibindo apenas produtos da categoria Phones |
| **Evidência** | [C03-CT02-filtro-phones.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C03-Catalogo-e-Filtros/C03-CT02-filtro-phones.png) |
| **Status** | ✅ Aprovado |

---

## C03-CT03 — Filtrar produtos por Laptops

| Campo | Detalhe |
|-------|---------|
| **ID** | C03-CT03 |
| **Descrição** | Verificar se o filtro de categoria Laptops exibe apenas notebooks |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E consigo ver todos os produtos listados |
| 3 | QUANDO clico na categoria "Laptops" no menu lateral |
| 4 | ENTÃO a lista deve ser atualizada |
| 5 | E devo ver apenas produtos da categoria Laptops |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | Apenas produtos da categoria Laptops devem aparecer após o filtro |
| **Resultado esperado** | Lista atualizada exibindo somente notebooks |
| **Resultado real** | Filtro aplicado corretamente, exibindo apenas produtos da categoria Laptops |
| **Evidência** | [C03-CT03-filtro-laptops.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C03-Catalogo-e-Filtros/C03-CT03-filtro-laptops.png) |
| **Status** | ✅ Aprovado |
---

## C03-CT04 — Filtrar produtos por Monitors

| Campo | Detalhe |
|-------|---------|
| **ID** | C03-CT04 |
| **Descrição** | Verificar se o filtro de categoria Monitors exibe apenas monitores |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E consigo ver todos os produtos listados |
| 3 | QUANDO clico na categoria "Monitors" no menu lateral |
| 4 | ENTÃO a lista deve ser atualizada |
| 5 | E devo ver apenas produtos da categoria Monitors |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | Apenas produtos da categoria Monitors devem aparecer após o filtro |
| **Resultado esperado** | Lista atualizada exibindo somente monitores |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |

---

## C03-CT05 — Voltar a exibir todos os produtos

| Campo | Detalhe |
|-------|---------|
| **ID** | C03-CT05 |
| **Descrição** | Verificar se é possível limpar o filtro e voltar a ver todos os produtos |
| **Pré-condições** | Um filtro de categoria deve estar aplicado |
| **Prioridade** | Média |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial com um filtro de categoria aplicado |
| 2 | QUANDO clico na opção "Categories" no menu lateral |
| 3 | ENTÃO a lista deve voltar a exibir todos os produtos disponíveis |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | Todos os produtos devem ser exibidos novamente após limpar o filtro |
| **Resultado esperado** | Lista completa de produtos visível sem filtro aplicado |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |
