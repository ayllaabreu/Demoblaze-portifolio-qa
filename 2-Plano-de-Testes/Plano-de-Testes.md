# Plano de Testes — DemoBlaze

## Objetivo

Esse documento descreve o que pretendo testar no DemoBlaze 
e como vou organizar esse trabalho. A ideia é cobrir as 
funcionalidades principais da loja e registrar tudo que 
encontrar ao longo da execução.

---

## O que vou testar

Vou focar nos fluxos que um usuário real usaria no dia a dia:

- Criar uma conta e fazer login
- Navegar pelo catálogo e filtrar por categoria
- Acessar a página de um produto
- Adicionar e remover produtos do carrinho
- Finalizar uma compra
- Enviar uma mensagem pelo formulário de contato

## O que não vou testar

- Performance e tempo de carregamento
- Segurança e vulnerabilidades
- Acesso pelo celular ou tablet
- A seção "About Us"

---

## Ambiente de teste

| Item | Detalhe |
|------|---------|
| URL | https://www.demoblaze.com |
| Navegador | Google Chrome 151.0.7922.76 (Versão oficial) |
| Sistema Operacional | Windows 11 64 bits |
| Tipo de teste | Manual e exploratório |

---

## Tipos de teste que vou aplicar

**Teste funcional** — verificar se cada funcionalidade 
faz o que deveria fazer.

**Teste de caminho feliz (happy path)** — seguir o fluxo 
ideal do usuário sem nenhum erro intencional.

**Teste negativo** — tentar ações inesperadas, como deixar 
campos vazios, inserir dados inválidos e ver como o sistema 
reage.

**Teste exploratório** — navegar livremente pelo site 
buscando comportamentos estranhos que não estejam nos 
cenários planejados.

---

## Critérios para começar os testes

- Site acessível e funcionando no navegador
- Cenários e casos de teste escritos
- Ambiente de captura de evidências pronto 
  (LICEcap instalado para gravar GIFs)

## Critérios para encerrar os testes

- Todos os casos de teste executados
- Bugs encontrados documentados com evidência
- Resultado de cada caso de teste preenchido 
  (aprovado ou reprovado)

---

## Como vou organizar a execução

Pretendo testar módulo por módulo, na ordem abaixo, 
começando sempre pelo caminho feliz antes de partir 
para os cenários negativos:

1. Cadastro
2. Login e Logout
3. Catálogo e Filtros
4. Página do Produto
5. Carrinho
6. Checkout
7. Formulário de Contato

---

## Ferramentas que vou usar

| Ferramenta | Para quê |
|-----------|---------|
| Google Chrome | Executar os testes |
| GitHub | Documentar e versionar o portfólio |
| Markdown | Escrever toda a documentação |
