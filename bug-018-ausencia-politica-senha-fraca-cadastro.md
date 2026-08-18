# [BUG-018] Ausência de validação de complexidade e aceitação de senhas fracas no cadastro

## 📌 Descrição Geral
No formulário de criação de conta (`/signup`), o campo de senha (*Password*) não aplica regras mínimas de segurança ou complexidade. A aplicação aceita o registro de senhas extremamente fracas e previsíveis (como `00000`), sem exigir um comprimento mínimo adequado ou combinação de caracteres, vulnerabilizando as contas dos usuários.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** Automation Exercise
* **URL:** `https://automationexercise.com/signup`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://automationexercise.com/`.
2. Clique em **Signup / Login** no menu superior.
3. Preencha Nome e E-mail válidos na seção *New User Signup!* e clique em **Signup**.
4. Na página de cadastro completo (`/signup`), insira a senha `00000` no campo **Password**.
5. Preencha os demais campos obrigatórios e clique em **Create Account**.
6. Observe o resultado da criação da conta.

---

## 🎯 Comportamento Esperado
* O sistema deve exigir uma política de senha forte (mínimo de 8 caracteres, incluindo letras, números e símbolos) e recusar sequências numéricas óbvias, exibindo um alerta orientativo de segurança ao usuário.

---

## ❌ Comportamento Atual (Bug)
* A aplicação valida e conclui a criação da conta aceitando a senha fraca `00000` sem emitir avisos ou restrições de segurança.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Vulnerabilidade de segurança na camada de autenticação).
* **Prioridade:** Média (Impacta a proteção de dados dos usuários cadastrados no sistema).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
