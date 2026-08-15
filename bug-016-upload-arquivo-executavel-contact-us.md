# [BUG-016] Ausência de validação de extensão e tipo de arquivo no upload do formulário Contact Us

## 📌 Descrição Geral
No formulário de suporte e contato (`/contact_us`), o campo de anexo de arquivos ("Upload File") não realiza a filtragem de extensões ou tipos MIME permitidos. A aplicação permite o envio com sucesso de arquivos executáveis (ex: `.exe`), expondo a plataforma a riscos de segurança e armazenamento indevido.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** Automation Exercise
* **URL:** `https://automationexercise.com/contact_us`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://automationexercise.com/`.
2. No menu superior, clique em **Contact us**.
3. Preencha os campos obrigatórios (*Name*, *Email*, *Subject* e *Message*).
4. No campo **Upload File**, selecione um arquivo com extensão executável (ex: `.exe`).
5. Clique no botão **Submit** e confirme o alerta de envio.

---

## 🎯 Comportamento Esperado
* O sistema deve restringir o upload apenas a formatos seguros e documentais (ex: `.pdf`, `.jpg`, `.png`), recusando arquivos `.exe` e exibindo uma mensagem de validação ao usuário.

---

## ❌ Comportamento Atual (Bug)
* A aplicação aceita o arquivo executável sem restrições e exibe a mensagem de confirmação: `"Success! Your details have been submitted successfully."`.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Alta (Falha de validação em upload que afeta a segurança e a integridade da aplicação).
* **Prioridade:** Alta (Requer implementação imediata de *whitelist* de extensões no upload).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
