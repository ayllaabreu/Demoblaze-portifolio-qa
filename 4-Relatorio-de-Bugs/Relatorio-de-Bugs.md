### BUG-001

| Campo | Detalhe |
|-------|---------|
| **Título** | [Catálogo] Categoria selecionada não é destacada visualmente no menu lateral |
| **Módulo** | Catálogo e Filtros |
| **Severidade** | 🟢 Baixa |
| **Status** | Aberto |

**Passos para reproduzir:**

| # | Passo |
|---|-------|
| 1 | DADO que estou na página inicial do DemoBlaze |
| 2 | QUANDO clico em qualquer categoria no menu lateral (Phones, Laptops ou Monitors) |
| 3 | ENTÃO a categoria clicada não é destacada visualmente |
| 4 | E a URL não é atualizada para indicar a categoria selecionada |

| Campo | Detalhe |
|-------|---------|
| **Resultado esperado** | A categoria selecionada deve ser destacada visualmente e a URL deve refletir a navegação atual |
| **Resultado atual** | Nenhum destaque visual é aplicado à categoria selecionada e a URL permanece como demoblaze.com/# |
| **Evidência** | [BUG-001-categoria-sem-destaque.png](https://github.com/ayllaabreu/Demoblaze-portifolio-qa/blob/main/6-Evidencias/C03-Catalogo-e-Filtros/BUG-001-categoria-sem-destaque.png) |
