# [BUG-023] Ausência de validação e aceitação de dados puramente numéricos nos campos Nome e Sobrenome

## 📌 Descrição Geral
Na funcionalidade de tabela dinâmica (**Web Tables**), o formulário de adição de novos registros aceita entradas compostas exclusivamente por caracteres numéricos nos campos **First Name** e **Last Name**, sem disparar alertas de validação ou impedir o salvamento na tabela.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** DemoQA
* **URL:** `https://demoqa.com/webtables`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://demoqa.com/webtables`.
2. Clique no botão **Add** para abrir o formulário de cadastro (*Registration Form*).
3. No campo **First Name**, preencha com apenas números (ex: `12345`).
4. No campo **Last Name**, preencha com apenas números (ex: `67890`).
5. Preencha os demais campos obrigatórios (*Email*, *Age*, *Salary*, *Department*) com dados válidos.
6. Clique no botão **Submit**.
7. Observe o registro inserido na tabela.

---

## 🎯 Comportamento Esperado
* Os campos de nome e sobrenome devem possuir validação Regex para restringir a entrada a caracteres alfabéticos (e acentuações/espaços), exibindo uma mensagem de erro visual e impedindo a submissão caso sejam inseridos apenas números.

---

## ❌ Comportamento Atual (Bug)
* O formulário valida a submissão com sucesso e insere o novo registro contendo números nos campos de nome e sobrenome diretamente na tabela da interface.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Inconsistência de dados e ausência de sanitização de formulário).
* **Prioridade:** Média (Impacta a integridade dos dados armazenados e exibidos na plataforma).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
