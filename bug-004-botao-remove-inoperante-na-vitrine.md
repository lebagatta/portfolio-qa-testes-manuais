# [BUG-004] Botão "Remove" inoperante na página de vitrine após adicionar produto

## 📌 Descrição Geral
Na página de catálogo de produtos (`/inventory.html`), após o usuário adicionar um item ao carrinho, o botão altera seu estado visual para "Remove", porém não reage ao clique do usuário quando este tenta remover o item diretamente da vitrine. Para conseguir excluir o produto, o usuário é forçado a navegar até a tela do carrinho (`/cart.html`).

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/inventory.html`
* **Navegador:** Microsoft Edge / Google Chrome
* **Perfil do Usuário Logado:** `problem_user`

---

## 📋 Passos para Reproduzir
1. Acesse o site `https://www.saucedemo.com/`.
2. Realize o login com o usuário `problem_user` e a senha `secret_sauce`.
3. Na vitrine de produtos (`/inventory.html`), clique em **"Add to cart"** em um dos produtos disponíveis (ex: *Sauce Labs Backpack*).
4. Observe que o botão muda para **"Remove"** e o contador do carrinho passa a marcar `1`.
5. Tente clicar no botão **"Remove"** na própria página do catálogo para retirar o item do carrinho.

---

## 🎯 Comportamento Esperado
* O botão "Remove" deve responder ao clique do usuário.
* O estado do botão deve retornar para "Add to cart".
* O contador do ícone do carrinho deve ser decrementado (retornando a `0`).

---

## ❌ Comportamento Atual (Bug)
* O botão "Remove" fica inoperante/unresponsive na vitrine de produtos.
* O produto permanece no carrinho e o contador do ícone não altera.
* A remoção do produto só é possível se o usuário acessar a página do carrinho (`/cart.html`) e clicar em "Remove" por lá.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Prejudica a usabilidade e a fluidez de navegação do usuário).
* **Prioridade:** Média (Gera frustração no fluxo de compra, exigindo passos adicionais para uma ação simples).

---

## 📷 Evidências e Anexos
> *(Insira um print da tela com o produto marcado como "Remove" e o contador do carrinho sem alterar após o clique)*
> 
> `![Evidência do Bug 004](./imagens/evidencia-bug-004.png)`
