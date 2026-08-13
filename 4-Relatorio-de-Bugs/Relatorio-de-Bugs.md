### BUG-001

| Campo | Detalhe |
|-------|---------|
| **Título** | [Catálogo] Categoria selecionada não é destacada visualmente no menu lateral |
| **Ambiente** | Chrome 151.0.7922.109 (Versão oficial) 64 bits, Windows 11, demoblaze.com |
| **Módulo** | Catálogo e Filtros |
| **Severidade** | 🟢 Baixa |
| **Status** | Aberto |

**Passos para Reproduzir:**

| # | Passo |
|---|-------|
| 1 | Acessar demoblaze.com |
| 2 | Clicar em qualquer categoria no menu lateral |
| 3 | Observar o menu lateral e a URL após o clique |

| Campo | Detalhe |
|-------|---------|
| **Resultado Atual** | Nenhum destaque visual aplicado à categoria e URL permanece como demoblaze.com/# |
| **Resultado Esperado** | Categoria selecionada destacada visualmente e URL atualizada |
| **Evidência** | [BUG-001-categoria-sem-destaque.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C03-Catalogo-e-Filtros/BUG-001-categoria-sem-destaque.png) |

---

### BUG-002

| Campo | Detalhe |
|-------|---------|
| **Título** | [Carrinho] Botão "Place Order" permanece visível com carrinho vazio e total não é exibido |
| **Ambiente** | Chrome 151.0.7922.109 (Versão oficial) 64 bits, Windows 11, demoblaze.com |
| **Módulo** | Carrinho |
| **Severidade** | 🔴 Alta |
| **Status** | Aberto |

**Passos para Reproduzir:**

| # | Passo |
|---|-------|
| 1 | Acessar demoblaze.com |
| 2 | Clicar em "Cart" no menu sem ter adicionado nenhum produto |
| 3 | Observar que o total não é exibido e o botão "Place Order" está visível |
| 4 | Clicar em "Place Order" |
| 5 | Observar que o formulário de pedido abre mesmo sem produtos no carrinho |

| Campo | Detalhe |
|-------|---------|
| **Resultado Atual** | Carrinho fica vazio sem exibir mensagem de "carrinho vazio", total desaparece, botão "Place Order" permanece visível e ao clicar abre o formulário de pedido mesmo sem produtos no carrinho |
| **Resultado Esperado** | Sistema deve exibir mensagem informando que o carrinho está vazio e desabilitar ou ocultar o botão "Place Order" |
| **Evidência** | [Carrinho vazio sem total](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT05-carrinho-vazio.png) / [Formulário aberto sem produtos](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT05-place-order-carrinho-vazio.png) |

---

### BUG-003

| Campo | Detalhe |
|-------|---------|
| **Título** | [Checkout] Data exibida na confirmação do pedido não corresponde ao mês informado no formulário |
| **Ambiente** | Chrome 151.0.7922.109 (64 bits), Windows 11, demoblaze.com |
| **Módulo** | Checkout |
| **Severidade** | 🔴 Alta |
| **Status** | Aberto |

**Passos para Reproduzir:**

| # | Passo |
|---|-------|
| 1 | Acessar demoblaze.com e fazer login |
| 2 | Adicionar um produto ao carrinho |
| 3 | Clicar em "Place Order" |
| 4 | Preencher o campo "Month" com "08" |
| 5 | Preencher os demais campos corretamente |
| 6 | Clicar em "Purchase" |
| 7 | Observar a data exibida na confirmação |

| Campo | Detalhe |
|-------|---------|
| **Resultado Atual** | Data exibida na confirmação mostra mês 7 em vez do mês 08 informado no formulário |
| **Resultado Esperado** | Data exibida deve corresponder exatamente ao mês informado no formulário |
| **Evidência** | [Item no carrinho logado](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT02-1-item-carrinho-logado.png) / [Place Order preenchido](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT02-2-place-order-preenchido.png) / [Confirmação do pedido](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT02-3-confirmacao-pedido.png)|

---

### BUG-004

| Campo | Detalhe |
|-------|---------|
| **Título** | [Checkout] Campos do formulário "Place Order" permanecem editáveis após confirmação da compra |
| **Ambiente** | Chrome 151.0.7922.109 (64 bits), Windows 11, demoblaze.com |
| **Módulo** | Checkout |
| **Severidade** | 🟡 Média |
| **Status** | Aberto |

**Passos para Reproduzir:**

| # | Passo |
|---|-------|
| 1 | Acessar demoblaze.com e fazer login |
| 2 | Adicionar um produto ao carrinho |
| 3 | Clicar em "Place Order" e preencher todos os campos |
| 4 | Clicar em "Purchase" |
| 5 | Observar que o popup de confirmação abre |
| 6 | Observar os campos do formulário visíveis atrás do popup |

| Campo | Detalhe |
|-------|---------|
| **Resultado Atual** | Os campos "Name" e "Year" do formulário permanecem visíveis e editáveis atrás do popup de confirmação da compra |
| **Resultado Esperado** | Após a confirmação da compra o formulário deve ser bloqueado ou ocultado completamente |
| **Evidência** | [Item no carrinho logado](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT02-1-item-carrinho-logado.png) / [Place Order preenchido](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT02-2-place-order-preenchido.png) / [Confirmação do pedido](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT02-3-confirmacao-pedido.png)|

---

### BUG-005

| Campo | Detalhe |
|-------|---------|
| **Título** | [Checkout] Usuário concluí compra sem estar logado |
| **Ambiente** | Chrome 151.0.7922.109 (64 bits), Windows 11, demoblaze.com |
| **Módulo** | Checkout |
| **Severidade** | 🔴 Alta |
| **Status** | Aberto |

**Passos para Reproduzir:**

| # | Passo |
|---|-------|
| 1 | Acessar demoblaze.com |
| 2 | Adicionar um produto ao carrinho |
| 3 | Clicar em "Place Order" e preencher todos os campos |
| 4 | Clicar em "Purchase" |
| 5 | Observar que o popup de confirmação abre |

| Campo | Detalhe |
|-------|---------|
| **Resultado Atual** | Pedido de compra é confirmado sem o usuário estar logado na plataforma |
| **Resultado Esperado** | Bloqueio da compra ou redirecionamento para o login |
| **Evidência** | [Item no carrinho sem login](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT03-1-item-carrinho-sem-login.png) / [Place Order preenchido](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT03-2-place-order-preenchido.png) / [Confirmação do pedido sem login](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C06-Checkout/C06-CT03-3-confirmacao-pedido-sem-login.png)|
