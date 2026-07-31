# [BUG-006] Inoperância dos botões de Adição e Remoção de produtos na vitrine

## 📌 Descrição Geral
Na vitrine de produtos (`/inventory.html`), ocorrem múltiplos comportamentos anômalos nos botões de ação dos cards: alguns produtos possuem o botão "Add to cart" inoperante ao clique, enquanto produtos que conseguem ser adicionados exibem o botão "Remove" que não reage à tentativa de remoção direta pela vitrine, forçando o usuário a acessar a página do carrinho para excluir o item.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/inventory.html`
* **Navegador:** Microsoft Edge / Google Chrome
* **Perfil do Usuário Logado:** `error_user`

---

## 📋 Passos para Reproduzir
1. Acesse `https://www.saucedemo.com/`.
2. Realize o login com o usuário `error_user` e senha `secret_sauce`.
3. Tente adicionar todos os produtos exibidos na vitrine ao carrinho.
4. Observe que determinados itens não reagem ao clique no botão **"Add to cart"**.
5. Nos itens que foram adicionados com sucesso, tente clicar no botão **"Remove"** para retirar o item do carrinho sem sair da vitrine.

---

## 🎯 Comportamento Esperado
* Todos os botões "Add to cart" devem permitir a adição do item ao carrinho.
* O botão "Remove" deve permitir a remoção imediata do produto diretamente na página de catálogo.

---

## ❌ Comportamento Atual (Bug)
* Produtos específicos possuem o botão "Add to cart" travado/inoperante.
* O botão "Remove" na vitrine não altera o estado do produto nem decrementa o contador do carrinho.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Alta (Impede a adição de determinados itens e dificulta a gestão do carrinho).
* **Prioridade:** Alta (Afeta diretamente o fluxo primário de conversão de compras).

---

