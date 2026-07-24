# [BUG-002] Botão "Add to cart" inoperante em produtos específicos da vitrine

## 📌 Descrição Geral
Ao navegar pela página principal de produtos (`/inventory.html`), diversos itens apresentam botões "Add to cart" que não reagem ao clique do usuário. Dos 6 produtos disponíveis na vitrine, apenas 3 permitem a adição ao carrinho de compras, impedindo a conversão de vendas dos demais itens.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/inventory.html`
* **Navegador:** Microsoft Edge (Versão mais recente)
* **Sistema Operacional:** Windows 10 / 11
* **Perfil do Usuário Logado:** `problem_user`

---

## 📋 Passos para Reproduzir
1. Acesse o site `https://www.saucedemo.com/` no Microsoft Edge.
2. Realize o login com o usuário `problem_user` e a senha `secret_sauce`.
3. Na vitrine de produtos (`/inventory.html`), tente clicar sequencialmente no botão **"Add to cart"** de todos os 6 produtos da lista:
   * *Sauce Labs Backpack*
   * *Sauce Labs Bike Light*
   * *Sauce Labs Bolt T-Shirt*
   * *Sauce Labs Fleece Jacket*
   * *Sauce Labs Onesie*
   * *Test.allTheThings() T-Shirt (Red)*
4. Observe o contador do badge do carrinho no canto superior direito e a alteração dos botões para "Remove".

---

## 🎯 Comportamento Esperado
* Todos os 6 botões "Add to cart" devem responder ao clique do usuário.
* O estado do botão deve alternar para "Remove".
* O contador do ícone do carrinho deve incrementar individualmente a cada item adicionado, atingindo o total de `6`.

---

## ❌ Comportamento Atual (Bug)
* O sistema permite a adição de apenas **3 produtos específicos** ao carrinho.
* Os outros 3 produtos não reagem ao evento de clique no botão "Add to cart": o botão não altera seu estado e o contador do carrinho não é incrementado, mesmo após sucessivas tentativas e recarregamento de página.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Alta (Bloqueia o fluxo principal de vendas de metade do catálogo de produtos).
* **Prioridade:** Alta (Impede a finalização de compra de itens do e-commerce).

---

## 📷 Evidências e Anexos
> *(Insira um print demonstrando a página com os botões clicados e o contador do carrinho marcando apenas 3 itens)*
> 
> `![Evidência do Bug 002](./imagens/evidencia-bug-002.png)`
