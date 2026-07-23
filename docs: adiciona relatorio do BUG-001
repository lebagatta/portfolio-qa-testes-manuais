# [BUG-001] Filtro de ordenação alfabética (A-Z e Z-A) não respeita a ordem dos produtos na vitrine

## 📌 Descrição Geral
Ao aplicar os filtros de ordenação "Name (A to Z)" ou "Name (Z to A)" na página de produtos (`/inventory.html`), a listagem de itens é exibida de forma desordenada/embaralhada, não respeitando a regra de negócio da ordenação alfabética.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/inventory.html`
* **Navegador:** Microsoft Edge (Versão mais recente)
* **Sistema Operacional:** Windows 10 / 11
* **Perfil do Usuário Logado:** `standard_user` / `problem_user`

---

## 📋 Passos para Reproduzir
1. Acesse o site `https://www.saucedemo.com/` através do navegador Microsoft Edge.
2. Realize o login preenchendo as credenciais válidas e clique em **Login**.
3. Na página principal de produtos (`/inventory.html`), localize o menu suspenso (dropdown) de ordenação no canto superior direito.
4. Selecione a opção **Name (A to Z)**.
5. Observe a sequência do nome dos produtos listados.
6. Altere a seleção para a opção **Name (Z to A)** e observe novamente.

---

## 🎯 Comportamento Esperado
* Ao selecionar **Name (A to Z)**, os produtos devem ser organizados estritamente em ordem alfabética ascendente (ex: *Sauce Labs Backpack* -> *Sauce Labs Bike Light* -> *Sauce Labs Bolt T-Shirt*...).
* Ao selecionar **Name (Z to A)**, os produtos devem ser organizados em ordem alfabética descendente.

---

## ❌ Comportamento Atual (Bug)
* Os produtos permanecem em uma ordem aleatória/embaralhada, ignorando o critério alfabético selecionado.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Afeta a usabilidade e a experiência de compra do usuário na vitrine).
* **Prioridade:** Média (Funcionalidade secundária de navegação, mas essencial para e-commerce).

---

## 📷 Evidências e Anexos
> *(Dica de Portfólio: Tire um print da tela com o filtro selecionado e a lista embaralhada, salve a imagem na pasta do projeto e adicione o link aqui)*
> 
> `![Evidência do Bug](./imagens/evidencia-bug-001.png)`

---

## 🔍 Observação Adicional de Compatibilidade
* **Incompatibilidade de Navegador:** A aplicação não respondeu/não carregou adequadamente no Google Chrome durante os testes iniciais, sendo aberta com sucesso apenas no Microsoft Edge. Recomenda-se investigação técnica de cross-browser.
