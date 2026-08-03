# [BUG-007] Impossibilidade de finalizar a compra (Botão "Finish" inoperante no Checkout)

## 📌 Descrição Geral
No fluxo de conclusão de pedido (`/checkout-step-two.html`), o botão **"Finish"** encontra-se inoperante ou desabilitado para o clique. Ao tentar concluir a transação após preencher os dados de envio e revisar o resumo do pedido, a aplicação não processa a ordem de compra nem redireciona o usuário para a tela de confirmação (`/checkout-complete.html`).

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/checkout-step-two.html`
* **Navegador:** Microsoft Edge / Google Chrome
* **Perfil do Usuário Logado:** `error_user`

---

## 📋 Passos para Reproduzir
1. Realize o login com o usuário `error_user`.
2. Adicione ao menos um produto válido ao carrinho e acesse a tela do carrinho (`/cart.html`).
3. Clique em **"Checkout"**.
4. Preencha os campos obrigatórios (*First Name*, *Last Name*, *Zip/Postal Code*) e clique em **"Continue"**.
5. Na tela de resumo do pedido (`Overview`), clique no botão **"Finish"**.

---

## 🎯 Comportamento Esperado
* O sistema deve processar o pedido, limpar o carrinho e redirecionar o usuário para a página de sucesso com a mensagem "Thank you for your order!".

---

## ❌ Comportamento Atual (Bug)
* O botão "Finish" não responde aos cliques do usuário, mantendo a tela estática no passo 2 do checkout e impedindo a conversão da compra.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Crítica (Bloqueia totalmente o funil de vendas da aplicação).
* **Prioridade:** Alta (Impossibilita a conclusão de pedidos na plataforma).

---

## 📷 Evidências e Anexos
> `![Evidência do Bug 007](./imagens/evidencia-bug-007.png)`
