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
| **Severidade** | 🟡 Média |
| **Status** | Aberto |

**Passos para Reproduzir:**

| # | Passo |
|---|-------|
| 1 | Acessar demoblaze.com |
| 2 | Adicionar qualquer produto ao carrinho |
| 3 | Acessar o carrinho |
| 4 | Clicar em "Delete" para remover o produto |

| Campo | Detalhe |
|-------|---------|
| **Resultado Atual** | Carrinho fica vazio sem exibir mensagem de "carrinho vazio", total desaparece e botão "Place Order" permanece visível |
| **Resultado Esperado** | Sistema deve exibir mensagem informando que o carrinho está vazio e desabilitar ou ocultar o botão "Place Order" |
| **Evidência** | [C05-CT05-carrinho-vazio.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT05-carrinho-vazio.png) / [Formulário aberto sem produtos](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT05-place-order-carrinho-vazio.png) |

