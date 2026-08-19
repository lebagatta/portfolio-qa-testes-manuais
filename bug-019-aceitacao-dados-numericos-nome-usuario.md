# [BUG-019] Ausência de validação de tipo de dado e aceitação de caracteres numéricos no campo de nome

## 📌 Descrição Geral
No formulário de cadastro de novos clientes do ParaBank (`/register.htm`), os campos "First Name" e "Last Name" não possuem restrição para tipos de dados textuais. A aplicação permite o registro de usuários utilizando apenas caracteres numéricos (ex: `12345`), aceitando dados cadastrais inconsistentes para uma plataforma bancária.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** ParaBank (Internet Banking)
* **URL:** `https://parabank.parasoft.com/parabank/register.htm`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://parabank.parasoft.com/parabank/register.htm`.
2. No campo **First Name**, insira uma sequência numérica (ex: `12345`).
3. No campo **Last Name**, insira uma sequência numérica (ex: `67890`).
4. Preencha os demais campos obrigatórios com informações válidas.
5. Clique no botão **REGISTER**.
6. Observe a confirmação de criação de conta.

---

## 🎯 Comportamento Esperado
* Os campos de nome próprio devem aceitar apenas caracteres alfabéticos e acentuações, exibindo uma mensagem de erro de validação caso números ou caracteres especiais sejam inseridos.

---

## ❌ Comportamento Atual (Bug)
* O sistema processa o cadastro normalmente, exibindo a mensagem de boas-vindas *"Welcome 12345 67890"* e criando a conta no sistema bancário com nome numérico.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Inconsistência de dados cadastrais e falha em regras de validação de formulário).
* **Prioridade:** Média (Afeta a qualidade e a integridade da base de dados dos clientes).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
