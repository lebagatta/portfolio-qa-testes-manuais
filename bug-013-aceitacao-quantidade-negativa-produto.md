# [BUG-013] Permitida a adição de produtos com quantidade zero ou negativa ao carrinho

## 📌 Descrição Geral
Na página de detalhes do produto no site Automation Exercise, o campo de quantidade (*Quantity*) não possui validação de limites inferiores para entradas do usuário. A aplicação permite a inserção de valores iguais a zero (`0`) ou números negativos (ex: `-1`), permitindo que o usuário adicione esses itens ao carrinho de compras e comprometendo o cálculo do subtotal do pedido.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** Automation Exercise
* **URL:** `https://automationexercise.com/product_details/1`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://automationexercise.com/`.
2. Clique na seção **Products** no menu superior.
3. Clique em **View Product** em qualquer item do catálogo.
4. No campo **Quantity**, altere o valor padrão `1` para `-1` (ou `0`).
5. Clique no botão **Add to cart**.
6. No modal de confirmação, clique em **View Cart**.
7. Observe a listagem de produtos e o cálculo total da compra.

---

## 🎯 Comportamento Esperado
* O campo de quantidade deve aceitar apenas inteiros positivos maiores que zero ($\ge 1$). 
* Caso o usuário tente inserir zero ou valores negativos, o sistema deve impedir a adição ao carrinho e exibir uma mensagem de validação como: *"A quantidade deve ser de no mínimo 1 unidade"*.

---

## ❌ Comportamento Atual (Bug)
* A aplicação aceita a entrada do valor negativo/zero, adiciona o produto ao carrinho e exibe a quantidade inválida na tabela de checkout, afetando a integridade dos dados e do cálculo total do pedido.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Alta (Inconsistência nos cálculos financeiros e na lógica do carrinho de compras).
* **Prioridade:** Alta (Falha em regra de negócio fundamental de um e-commerce).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
