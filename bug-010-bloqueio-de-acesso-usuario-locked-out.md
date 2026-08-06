# [BUG-010] Falha de autenticação e bloqueio de acesso no login (locked_out_user)

## 📌 Descrição Geral
Ao tentar realizar a autenticação na plataforma utilizando as credenciais cadastradas para o perfil `locked_out_user`, a aplicação impede o login e retém o usuário na página inicial (`index.html`), exibindo uma mensagem de bloqueio e impossibilitando o acesso à vitrine do sistema.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/`
* **Navegador:** Microsoft Edge / Google Chrome
* **Perfil do Usuário Logado:** `locked_out_user`

---

## 📋 Passos para Reproduzir
1. Acesse `https://www.saucedemo.com/`.
2. Insira o usuário `locked_out_user` no campo de usuário.
3. Insira a senha `secret_sauce` no campo de senha.
4. Clique no botão **"Login"**.
5. Observe o comportamento da aplicação e a notificação exibida.

---

## 🎯 Comportamento Esperado
* Para usuários ativos, a aplicação deve realizar a autenticação e redirecionar para `/inventory.html`. 
* Para contas com restrição/bloqueadas, o sistema deve exibir de forma clara a notificação de conta bloqueada sem travar o fluxo da aplicação.

---

## ❌ Comportamento Atual (Validação de Regra)
* O login é recusado e a aplicação exibe o alerta: `"Epic sadface: Sorry, this user has been locked out."`, mantendo a tela estática no formulário de acesso.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Alta (Impede completamente o acesso à plataforma para o usuário).
* **Prioridade:** Média (Validação de regra de negócio referente ao controle de acessos de usuários bloqueados).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
