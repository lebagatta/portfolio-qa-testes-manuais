# [BUG-011] Renderização incorreta e duplicada das imagens de produtos na vitrine

## 📌 Descrição Geral
Ao navegar pela vitrine de produtos (`/inventory.html`) utilizando o perfil `problem_user`, todas as imagens de capa dos produtos são substituídas incorretamente pela mesma imagem padrão (imagem de um cão com óculos / erro 404). As ilustrações originais das mercadorias não são carregadas, prejudicando o catálogo visual.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/inventory.html`
* **Navegador:** Microsoft Edge / Google Chrome
* **Perfil do Usuário Logado:** `problem_user`

---

## 📋 Passos para Reproduzir
1. Acesse `https://www.saucedemo.com/`.
2. Realize o login com o usuário `problem_user` e a senha `secret_sauce`.
3. Observe as imagens dos cards de cada produto na vitrine (`Sauce Labs Backpack`, `Sauce Labs Bike Light`, `Sauce Labs Bolt T-Shirt`, etc.).

---

## 🎯 Comportamento Esperado
* Cada card de produto deve exibir sua respectiva foto ilustrativa correspondente ao item anunciado.

---

## ❌ Comportamento Atual (Bug)
* Todos os cards de produtos exibem exatamente a mesma imagem duplicada (`/static/media/sl-404.168b1cce.jpg`), independente do produto listado.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Não impede a compra, mas afeta criticamente a experiência visual e de e-commerce).
* **Prioridade:** Média (Prejudica a apresentação da marca e o reconhecimento visual dos produtos pelo cliente).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
