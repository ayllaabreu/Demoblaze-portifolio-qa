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
| **Evidência** | [Data incorreta na confirmação](link-BUG-003-data-incorreta-confirmacao.png) |
