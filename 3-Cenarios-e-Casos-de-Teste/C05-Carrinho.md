# Cenário 05 - Carrinho

**Descrição:** Esse módulo cobre os testes do carrinho de 
compras do DemoBlaze. Validei desde a adição de produtos 
até a remoção, passando pela verificação do total e pelo 
comportamento do carrinho para usuários não logados.

---

## C05-CT01 - Adicionar um produto ao carrinho

| Campo | Detalhe |
|-------|---------|
| **ID** | C05-CT01 |
| **Descrição** | Verificar se é possível adicionar um produto ao carrinho |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página de detalhes de um produto |
| 2 | E consigo ver o botão "Add to cart" |
| 3 | QUANDO clico no botão "Add to cart" |
| 4 | ENTÃO devo ver uma confirmação de que o produto foi adicionado |
| 5 | E ao acessar o carrinho o produto deve aparecer na lista |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O produto deve aparecer no carrinho após ser adicionado |
| **Resultado esperado** | Confirmação de adição exibida e produto listado no carrinho |
| **Resultado real** | Mensagem "Product added" exibida e Nexus 6 aparece corretamente no carrinho |
| **Evidência** | [C05-CT01-adicionar-produto.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT01-adicionar-produto.png) / [C05-CT01-produto-no-carrinho.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT01-produto-no-carrinho.png) |
| **Status** | ✅ Aprovado |

---

## C05-CT02 - Adicionar mais de um produto ao carrinho

| Campo | Detalhe |
|-------|---------|
| **ID** | C05-CT02 |
| **Descrição** | Verificar se o carrinho aceita múltiplos produtos de categorias diferentes |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E acesso a página de um produto e clico em "Add to cart" |
| 3 | E volto ao catálogo e acesso um segundo produto diferente |
| 4 | QUANDO clico em "Add to cart" no segundo produto |
| 5 | ENTÃO ao acessar o carrinho os dois produtos devem aparecer na lista |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | Todos os produtos adicionados devem estar listados no carrinho |
| **Resultado esperado** | Carrinho exibindo os dois produtos corretamente |
| **Resultado real** | Nexus 6 e iPhone 6 32gb aparecem corretamente no carrinho após adição |
| **Evidência** | [C05-CT02-CT03-multiplos-produtos-total.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT02-CT03-multiplos-produtos-total.png) |
| **Status** | ✅ Aprovado |

---

## C05-CT03 - Verificar o total do carrinho

| Campo | Detalhe |
|-------|---------|
| **ID** | C05-CT03 |
| **Descrição** | Verificar se o valor total exibido no carrinho corresponde à soma dos produtos adicionados |
| **Pré-condições** | Ter pelo menos dois produtos no carrinho |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que tenho dois ou mais produtos adicionados ao carrinho |
| 2 | QUANDO acesso o carrinho |
| 3 | ENTÃO devo ver o preço individual de cada produto |
| 4 | E o valor total deve ser igual à soma de todos os produtos listados |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O total deve refletir corretamente a soma dos preços dos produtos no carrinho |
| **Resultado esperado** | Total calculado e exibido corretamente |
| **Resultado real** | Total exibido corretamente: Nexus 6 ($650) + iPhone 6 32gb ($790) = $1440 |
| **Evidência** | [C05-CT02-CT03-multiplos-produtos-total.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT02-CT03-multiplos-produtos-total.png) |
| **Status** | ✅ Aprovado |

---

## C05-CT04 - Remover um produto do carrinho

| Campo | Detalhe |
|-------|---------|
| **ID** | C05-CT04 |
| **Descrição** | Verificar se é possível remover um produto do carrinho e se o total é atualizado |
| **Pré-condições** | Ter pelo menos um produto no carrinho |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou no carrinho com pelo menos um produto listado |
| 2 | QUANDO clico em "Delete" ao lado do produto que quero remover |
| 3 | ENTÃO o produto deve desaparecer da lista |
| 4 | E o valor total deve ser atualizado automaticamente |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O produto removido não deve mais aparecer no carrinho e o total deve ser recalculado |
| **Resultado esperado** | Produto removido e total atualizado corretamente |
| **Resultado real** | Nexus 6 removido com sucesso. Total atualizado de $1440 para $790 |
| **Evidência** | [Antes de remover o Nexus](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT02-CT03-multiplos-produtos-total.png) / [Depois de remover o Nexus](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT04-remover-produto.png) |
| **Status** | ✅ Aprovado |

---

## C05-CT05 - Verificar carrinho vazio após remover todos os produtos

| Campo | Detalhe |
|-------|---------|
| **ID** | C05-CT05 |
| **Descrição** | Verificar o comportamento do carrinho quando todos os produtos são removidos |
| **Pré-condições** | Ter pelo menos um produto no carrinho |
| **Prioridade** | Média |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou no carrinho com um produto listado |
| 2 | QUANDO clico em "Delete" para remover o único produto |
| 3 | ENTÃO o carrinho deve ficar vazio |
| 4 | E o total deve ser zerado ou não exibido |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O carrinho deve indicar que está vazio de forma clara |
| **Resultado esperado** | Carrinho vazio exibido sem erros visuais |
| **Resultado real** | iPhone 6 removido com sucesso, porém o carrinho não exibe mensagem de "carrinho vazio" e o botão "Place Order" permanece visível sem produtos |
| **Evidência** | [C05-CT05-carrinho-vazio.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C05-Carrinho/C05-CT05-carrinho-vazio.png) |
| **Status** | ❌ Reprovado |

---

## C05-CT06 - Acessar o carrinho sem estar logada

| Campo | Detalhe |
|-------|---------|
| **ID** | C05-CT06 |
| **Descrição** | Verificar se é possível adicionar produtos e acessar o carrinho sem estar logada |
| **Pré-condições** | Não estar logada no sistema |
| **Prioridade** | Média |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que não estou logada no DemoBlaze |
| 2 | E acesso a página de detalhes de um produto |
| 3 | QUANDO clico em "Add to cart" |
| 4 | E acesso o carrinho pelo menu |
| 5 | ENTÃO o produto deve aparecer no carrinho mesmo sem estar logada |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve permitir adicionar ao carrinho sem login, conforme mapeado nos requisitos |
| **Resultado esperado** | Produto visível no carrinho sem necessidade de autenticação |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |
