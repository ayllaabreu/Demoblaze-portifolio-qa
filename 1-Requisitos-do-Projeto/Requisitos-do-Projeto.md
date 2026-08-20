# Requisitos do Projeto - DemoBlaze

## Sobre o Sistema

O DemoBlaze é uma loja virtual de demonstração criada para 
prática de testes manuais. Vende produtos eletrônicos como 
celulares, laptops e monitores. Explorei o site antes de 
começar os testes para entender como ele funciona e mapear 
o que seria testado.

**URL:** https://www.demoblaze.com  
**Tipo:** Aplicação web  
**Idioma:** Inglês  

---

## O que o sistema faz

### Cadastro e Login
- Novos usuários podem criar uma conta com username e senha
- Não é possível cadastrar um username que já existe
- Depois de logado, o nome do usuário aparece no menu
- É possível fazer logout a qualquer momento

### Catálogo de Produtos
- A página inicial mostra os produtos disponíveis
- Dá para filtrar por categoria: Phones, Laptops e Monitors
- Ao clicar em um produto, abre uma página com foto, 
  descrição e preço

### Carrinho
- Qualquer pessoa pode adicionar produtos ao carrinho, 
  mesmo sem estar logada
- O carrinho mostra os produtos adicionados e calcula 
  o total automaticamente
- É possível remover produtos do carrinho

### Checkout
- Para finalizar a compra, o usuário precisa estar logado
- O formulário pede: nome, país, cidade, número do cartão, 
  mês e ano
- Depois de confirmar, aparece uma mensagem de pedido realizado

### Formulário de Contato
- Tem um formulário de contato com campos de e-mail, 
  nome e mensagem
- Após o envio, o sistema exibe uma confirmação

---

## Regras que identifiquei ao explorar o sistema

| ID | Regra |
|----|-------|
| RN-001 | Não precisa estar logado para navegar e adicionar ao carrinho |
| RN-002 | Precisa estar logado para finalizar a compra |
| RN-003 | Username duplicado não é permitido no cadastro |
| RN-004 | O total do carrinho deve refletir corretamente a soma dos produtos |

---

## Fluxo principal que vou testar
→ Acessar o site
→ Criar conta
→ Fazer login
→ Navegar pelo catálogo
→ Abrir página do produto
→ Adicionar ao carrinho
→ Conferir o carrinho
→ Finalizar pedido
→ Confirmar compra

---

## O que não vou testar nesse projeto

- Performance do site
- Segurança
- Acesso pelo celular
- A seção "About Us"
