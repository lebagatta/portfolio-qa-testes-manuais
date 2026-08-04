# [BUG-008] Exceção de sistema e mensagem de erro ao acionar filtro de ordenação

## 📌 Descrição Geral
Ao tentar utilizar o seletor de ordenação de produtos na vitrine (`/inventory.html`), a aplicação dispara uma mensagem de alerta do sistema informando a quebra do componente de ordenação (`"Sorting is broken! This error has been reported to Backtrace."`), impedindo a reordenação da lista de produtos.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/inventory.html`
* **Navegador:** Microsoft Edge / Google Chrome
* **Perfil do Usuário Logado:** `error_user`

---

## 📋 Passos para Reproduzir
1. Acesse `https://www.saucedemo.com/`.
2. Realize o login com o usuário `error_user` e a senha `secret_sauce`.
3. Na vitrine de produtos, clique no menu dropdown de ordenação no canto superior direito.
4. Selecione qualquer opção de filtro diferente da padrão (ex: *Price (low to high)* ou *Name (Z to A)*).
5. Observe a caixa de diálogo/alerta exibida na tela.

---

## 🎯 Comportamento Esperado
* A listagem de produtos deve ser reordenada de acordo com o critério escolhido sem emitir exceções ou pop-ups de erro técnico para o usuário final.

---

## ❌ Comportamento Atual (Bug)
* A aplicação exibe um alerta modal com a mensagem: `"Sorting is broken! This error has been reported to Backtrace."` e a ordenação dos produtos não é aplicada.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Apresenta exceções e mensagens técnicas diretamente na interface do usuário).
* **Prioridade:** Média (Prejudica a navegabilidade e a filtragem no catálogo de produtos).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
