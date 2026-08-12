# [BUG-014] Ausência de validação de domínio completo de e-mail no formulário de Newsletter

## 📌 Descrição Geral
No rodapé de todas as páginas da aplicação, o campo de cadastro de Newsletter ("SUBSCRIPTION") valida apenas a presença do caractere `@`, permitindo a submissão de endereços de e-mail sem domínio válido ou extensão (ex: `ola@ola` ou `teste@teste`). A aplicação aceita a entrada e confirma a inscrição indevidamente.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** Automation Exercise
* **URL:** `https://automationexercise.com/`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://automationexercise.com/`.
2. Role a página até o rodapé (seção "SUBSCRIPTION").
3. No campo de entrada de e-mail, insira um endereço sem extensão de domínio (ex: `ola@ola`).
4. Clique no botão com a seta verde para enviar.
5. Observe a notificação de confirmação exibida.

---

## 🎯 Comportamento Esperado
* O formulário deve exigir um padrão de e-mail válido (ex: `nome@dominio.com`), exibindo uma mensagem de erro ao identificar domínios incompletos.

---

## ❌ Comportamento Atual (Bug)
* A aplicação processa a requisição e exibe a mensagem de sucesso `"You have been successfully subscribed!"`, gravando um e-mail sem extensão válida na base de dados.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Baixa (Não impede a navegação principal, mas gera inconsistência na base de contatos).
* **Prioridade:** Média (Prejudica a taxa de entrega e a integridade de disparos de e-mail marketing).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
