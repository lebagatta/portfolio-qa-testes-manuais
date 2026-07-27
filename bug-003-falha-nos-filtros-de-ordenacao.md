# [BUG-003] Inoperância total dos filtros de ordenação de produtos (Nome e Preço)

## 📌 Descrição Geral
Na tela de vitrine de produtos (`/inventory.html`), o componente de seleção de ordenação (dropdown) não aplica nenhuma regra de filtragem na lista. Ao selecionar as opções de ordenação alfabética (A-Z ou Z-A) ou por valor (Low to High ou High to Low), a exibição dos produtos permanece inalterada, impedindo a visualização organizada do catálogo.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/inventory.html`
* **Navegador:** Microsoft Edge (ou Google Chrome)
* **Perfil do Usuário Logado:** `problem_user`

---

## 📋 Passos para Reproduzir
1. Acesse o site `https://www.saucedemo.com/`.
2. Realize o login com o usuário `problem_user` e a senha `secret_sauce`.
3. Na página inicial do catálogo (`/inventory.html`), localize o campo seletor no canto superior direito (*Name (A to Z)*).
4. Altere a seleção do filtro para cada uma das opções disponíveis:
   * **Name (Z to A)**
   * **Price (low to high)**
   * **Price (high to low)**
5. Observe a disposição dos cards de produtos na página.

---

## 🎯 Comportamento Esperado
* A lista de produtos deve se reorganizar dinamicamente conforme a regra do filtro selecionado:
  * Ordenar os nomes em ordem alfabética inversa (Z a A).
  * Ordenar os produtos do menor valor monetário para o maior.
  * Ordenar os produtos do maior valor monetário para o menor.

---

## ❌ Comportamento Atual (Bug)
* O seletor altera o texto visual exibido no dropdown, porém **a ordem dos produtos na tela permanece idêntica à ordem inicial padrão**, ignorando os eventos de reordenação por nome e preço.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Dificulta a navegação do usuário no catálogo de compras).
* **Prioridade:** Média (Impacta a experiência de usabilidade e busca por preço/alfabética).

---

## 📷 Evidências e Anexos
> *(Insira um print da tela com o filtro selecionado em "Price (low to high)" enquanto a lista permanece desordenada)*
> 
> `![Evidência do Bug 003](./imagens/evidencia-bug-003.png)`
