# Cenário 07 - Formulário de Contato

**Descrição:** Esse módulo valida o formulário de contato 
do DemoBlaze. Apesar de ser uma funcionalidade simples, 
testei diferentes situações para verificar como o sistema 
se comporta com campos vazios, dados inválidos e envio 
correto.

---

## C07-CT01 - Enviar mensagem com todos os campos preenchidos

| Campo | Detalhe |
|-------|---------|
| **ID** | C07-CT01 |
| **Descrição** | Verificar se é possível enviar uma mensagem preenchendo todos os campos corretamente |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | E clico em "Contact" no menu de navegação |
| 3 | E preencho o campo "Contact Email" com um e-mail válido |
| 4 | E preencho o campo "Contact Name" com meu nome |
| 5 | E preencho o campo "Message" com uma mensagem |
| 6 | QUANDO clico no botão "Send message" |
| 7 | ENTÃO devo ver uma mensagem confirmando que o contato foi enviado |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve confirmar o envio da mensagem após o clique em "Send message" |
| **Resultado esperado** | Mensagem de confirmação de envio exibida com sucesso |
| **Resultado real** | Mensagem de confirmação "Thanks for the mmessage!!" exibida com sucesso |
| **Evidência** | [Mensagem enviada)](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C07-Formulario-de-Contato/C07-CT01-mensagem-enviada.png) |
| **Status** | ⏳ Aprovado |

---

## C07-CT02 - Tentar enviar formulário com todos os campos vazios

| Campo | Detalhe |
|-------|---------|
| **ID** | C07-CT02 |
| **Descrição** | Verificar se o sistema impede o envio quando todos os campos estão vazios |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Alta |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que abri o formulário de contato |
| 2 | E deixei todos os campos em branco |
| 3 | QUANDO clico no botão "Send message" |
| 4 | ENTÃO o sistema deve me avisar que os campos precisam ser preenchidos |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve bloquear o envio e indicar os campos obrigatórios |
| **Resultado esperado** | Alerta de campo obrigatório exibido antes do envio |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |

---

## C07-CT03 - Tentar enviar formulário com e-mail inválido

| Campo | Detalhe |
|-------|---------|
| **ID** | C07-CT03 |
| **Descrição** | Verificar se o sistema valida o formato do e-mail antes de permitir o envio |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Média |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que abri o formulário de contato |
| 2 | E preencho o campo "Contact Email" com um texto sem formato de e-mail como "ayllateste" |
| 3 | E preencho os demais campos corretamente |
| 4 | QUANDO clico no botão "Send message" |
| 5 | ENTÃO o sistema deve me avisar que o e-mail informado é inválido |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve validar o formato do e-mail e bloquear o envio se estiver inválido |
| **Resultado esperado** | Mensagem de erro informando que o e-mail está em formato inválido |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |

---

## C07-CT04 - Tentar enviar formulário apenas com o campo mensagem vazio

| Campo | Detalhe |
|-------|---------|
| **ID** | C07-CT04 |
| **Descrição** | Verificar se o sistema impede o envio quando apenas o campo mensagem está vazio |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Média |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que abri o formulário de contato |
| 2 | E preencho o campo "Contact Email" com um e-mail válido |
| 3 | E preencho o campo "Contact Name" com meu nome |
| 4 | E deixo o campo "Message" em branco |
| 5 | QUANDO clico no botão "Send message" |
| 6 | ENTÃO o sistema deve me avisar que o campo mensagem precisa ser preenchido |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O sistema deve bloquear o envio quando o campo mensagem estiver vazio |
| **Resultado esperado** | Alerta indicando que o campo mensagem é obrigatório |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |

---

## C07-CT05 - Fechar o formulário de contato sem enviar

| Campo | Detalhe |
|-------|---------|
| **ID** | C07-CT05 |
| **Descrição** | Verificar se é possível fechar o formulário sem enviar e voltar à página normalmente |
| **Pré-condições** | Nenhuma |
| **Prioridade** | Baixa |

**Passos:**

| # | Passo |
|---|-------|
| 1 | DADO que abri o formulário de contato |
| 2 | E preenchi alguns campos mas decidi não enviar |
| 3 | QUANDO clico no botão "Close" ou no X do formulário |
| 4 | ENTÃO o formulário deve ser fechado |
| 5 | E devo continuar na página inicial sem nenhum erro |

| Campo | Detalhe |
|-------|---------|
| **Critérios de aceitação** | O formulário deve fechar sem erros e a página deve continuar funcionando normalmente |
| **Resultado esperado** | Formulário fechado e página inicial acessível sem erros |
| **Resultado real** | (preencher durante a execução) |
| **Evidência** | (inserir print ou GIF após execução) |
| **Status** | ⏳ Não executado |
