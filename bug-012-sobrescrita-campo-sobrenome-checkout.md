# [BUG-012] Apagamento automático e falha na retenção de texto no campo "Last Name" do Checkout

## 📌 Descrição Geral
Ao tentar preencher os dados de entrega na primeira etapa do checkout (`/checkout-step-one.html`), o campo de texto **"Last Name"** (Sobrenome) não retém o conteúdo digitado pelo usuário. Assim que os caracteres são inseridos, a aplicação apaga automaticamente o valor ou impede a persistência do texto, impossibilitando a submissão do formulário de compra.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/checkout-step-one.html`
* **Navegador:** Microsoft Edge / Google Chrome
* **Perfil do Usuário Logado:** `problem_user`

---

## 📋 Passos para Reproduzir
1. Acesse `https://www.saucedemo.com/`.
2. Realize o login com o usuário `problem_user` e a senha `secret_sauce`.
3. Adicione qualquer produto ao carrinho e navegue até a tela do carrinho (`/cart.html`).
4. Clique em **"Checkout"**.
5. No formulário de informações do comprador, tente digitar qualquer texto no campo **"Last Name"**.
6. Observe que o texto é apagado/resetado automaticamente.

---

## 🎯 Comportamento Esperado
* O campo "Last Name" deve aceitar a entrada de texto do usuário, manter os caracteres visíveis e permitir o avanço para a etapa de confirmação do pedido ao clicar em "Continue".

---

## ❌ Comportamento Atual (Bug)
* O texto digitado no campo "Last Name" é instantaneamente apagado pela aplicação. Como o campo é de preenchimento obrigatório, o sistema impede o prosseguimento do checkout, exibindo a mensagem de erro: *"Error: Last Name is required"*.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Alta (Impede o preenchimento de um campo obrigatório no checkout).
* **Prioridade:** Alta (Bloqueia totalmente o fluxo de conversão e fechamento de pedidos).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
