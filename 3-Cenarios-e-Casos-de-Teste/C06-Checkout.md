# Cenário 06 - Checkout

**Descrição:** Esse módulo valida o fluxo de finalização 
de compra do DemoBlaze. Testei o caminho completo de um 
pedido bem-sucedido e também situações como campos vazios 
e tentativa de compra sem estar logada — que é onde os 
comportamentos mais interessantes costumam aparecer.

---

## C06-CT01 - Finalizar compra com todos os campos preenchidos

| Campo | Detalhe |
|-------|---------|
| **ID** | C06-CT01 |
| **Descrição** | Verificar se é possível concluir uma compra preenchendo todos os campos do formulário |
| **Pré-condições** | Estar logada e ter pelo menos um produto no carrinho |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou logada e tenho produtos no carrinho |
| 2 | E estou na página do carrinho |
| 3 | QUANDO clico no botão "Place Order" |
| 4 | E preencho o campo "Name" com meu nome |
| 5 | E preencho o campo "Country" com meu país |
| 6 | E preencho o campo "City" com minha cidade |
| 7 | E preencho o campo "Credit card" com um número de cartão |
| 8 | E preencho os campos "Month" e "Year" |
| 9 | E clico no botão "Purchase" |
| 10 | ENTÃO devo ver uma mensagem confirmando que o pedido foi realizado |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve confirmar o pedido e exibir um resumo da compra |
| **Resultado esperado** | Mensagem de confirmação com os dados do pedido exibida com sucesso |
| **Resultado real** | Compra finalizada com sucesso. Mensagem "Thank you for your purchase!" exibida com ID 7932679, valor $700, nome Aylla e data 12/7/2026 |
| **Evidência** | [C06-CT01-compra-concluida.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT01-compra-concluida.png) |
| **Status** | ✅ Aprovado |

---

## C06-CT02 - Verificar informações exibidas na confirmação do pedido

| Campo | Detalhe |
|-------|---------|
| **ID** | C06-CT02 |
| **Descrição** | Verificar se a mensagem de confirmação exibe os dados corretos do pedido |
| **Pré-condições** | Ter concluído uma compra com sucesso |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que finalizei uma compra com sucesso |
| 2 | QUANDO a mensagem de confirmação é exibida |
| 3 | ENTÃO devo ver o valor total da compra |
| 4 | E devo ver o nome que informei no formulário |
| 5 | E devo ver um número ou identificador do pedido |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | A confirmação deve exibir pelo menos o valor total e o nome do comprador |
| **Resultado esperado** | Dados do pedido exibidos corretamente na tela de confirmação |
| **Resultado real** | Confirmação exibe ID, valor e nome corretamente, porém a data apresenta mês incorreto — bug registrado como BUG-003 |
| **Evidência** | |
| **Status** | ❌ Reprovado |

---

## C06-CT03 - Tentar finalizar compra sem estar logada

| Campo | Detalhe |
|-------|---------|
| **ID** | C06-CT03 |
| **Descrição** | Verificar o comportamento do sistema ao tentar finalizar uma compra sem autenticação |
| **Pré-condições** | Não estar logada e ter pelo menos um produto no carrinho |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que não estou logada no DemoBlaze |
| 2 | E tenho pelo menos um produto no carrinho |
| 3 | E estou na página do carrinho |
| 4 | QUANDO clico no botão "Place Order" |
| 5 | ENTÃO o sistema deve me impedir de concluir a compra |
| 6 | Ou devo ser redirecionada para a tela de login |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema não deve permitir finalizar a compra sem autenticação |
| **Resultado esperado** | Bloqueio da compra ou redirecionamento para o login |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |

---

## C06-CT04 - Tentar finalizar compra com campos obrigatórios vazios

| Campo | Detalhe |
|-------|---------|
| **ID** | C06-CT04 |
| **Descrição** | Verificar se o sistema impede a finalização da compra quando campos obrigatórios não são preenchidos |
| **Pré-condições** | Estar logada e ter pelo menos um produto no carrinho |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou logada e tenho produtos no carrinho |
| 2 | E cliquei em "Place Order" |
| 3 | E deixei todos os campos do formulário em branco |
| 4 | QUANDO clico no botão "Purchase" |
| 5 | ENTÃO o sistema deve me avisar que os campos obrigatórios precisam ser preenchidos |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve bloquear a compra e indicar quais campos precisam ser preenchidos |
| **Resultado esperado** | Alerta de campo obrigatório exibido antes de concluir a compra |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |

---

## C06-CT05 - Tentar finalizar compra com carrinho vazio

| Campo | Detalhe |
|-------|---------|
| **ID** | C06-CT05 |
| **Descrição** | Verificar o comportamento do sistema ao tentar finalizar uma compra sem produtos no carrinho |
| **Pré-condições** | Estar logada e o carrinho deve estar vazio |
| **Prioridade** | Média |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou logada no DemoBlaze |
| 2 | E o meu carrinho está vazio |
| 3 | QUANDO clico no botão "Place Order" |
| 4 | ENTÃO o sistema deve me avisar que não há produtos no carrinho |
| 5 | Ou o botão "Place Order" não deve estar disponível |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema não deve permitir finalizar uma compra sem produtos no carrinho |
| **Resultado esperado** | Aviso de carrinho vazio ou botão desabilitado |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |
