# [BUG-017] Falha no motor de busca e ausência de retorno para termos cadastrados no catálogo

## 📌 Descrição Geral
Na página de produtos (`/products`), o campo de pesquisa (*"Search Product"*) não retorna resultados para termos e palavras-chave que correspondem exatamente a itens cadastrados no catálogo. A busca resulta em uma página vazia ou sem retorno de dados, impedindo a localização de mercadorias pela barra de pesquisa.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** Automation Exercise
* **URL:** `https://automationexercise.com/products`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://automationexercise.com/`.
2. No menu superior, clique em **Products**.
3. No campo de busca **"Search Product"**, digite o nome de um produto existente no catálogo (ex: `Dress`, `Top` ou `Shirt`).
4. Clique no botão de pesquisa (ícone de lupa).
5. Observe o resultado retornado pela aplicação.

---

## 🎯 Comportamento Esperado
* O sistema deve realizar a busca no banco de dados e exibir todos os produtos cujos títulos ou categorias contenham o termo pesquisado.

---

## ❌ Comportamento Atual (Bug)
* A aplicação não retorna nenhum produto referente à pesquisa efetuada, exibindo uma listagem vazia mesmo para termos com correspondência exata nos itens cadastrados.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Alta (Inoperância de funcionalidade principal de navegação e localização de produtos).
* **Prioridade:** Alta (Impacta diretamente a experiência de compra e o funil de vendas do e-commerce).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
