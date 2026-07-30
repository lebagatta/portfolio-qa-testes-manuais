# [BUG-005] Alta latência e gargalo de desempenho no carregamento e navegação

## 📌 Descrição Geral
Ao utilizar a aplicação com o perfil de usuário específico, a plataforma apresenta atrasos severos (*delays*) no tempo de resposta das requisições e transições de tela. A navegação perde fluidez ao realizar o login e ao carregar a página de vitrine de produtos (`/inventory.html`), degradando a experiência do usuário.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/`
* **Navegador:** Microsoft Edge / Google Chrome
* **Perfil do Usuário Logado:** `performance_glitch_user`

---

## 📋 Passos para Reproduzir
1. Acesse o site `https://www.saucedemo.com/`.
2. Insira o usuário `performance_glitch_user` e a senha `secret_sauce`.
3. Clique no botão **"Login"**.
4. Observe o tempo de resposta para a autenticação e o carregamento completo da página de catálogo (`/inventory.html`).
5. Navegue entre as seções ou tente adicionar produtos ao carrinho.

---

## 🎯 Comportamento Esperado
* A autenticação de login e o carregamento dos elementos do catálogo devem ocorrer de forma fluida e responsiva (idealmente em menos de 1 a 2 segundos em conexões estáveis).

---

## ❌ Comportamento Atual (Bug)
* Ocorre um atraso significativo (*delay* de múltiplos segundos) para processar o login e renderizar a vitrine.
* A interface congela momentaneamente durante as requisições, gerando perda de fluidez visual e sensação de inoperância para o usuário.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Afeta diretamente o desempenho percebido e a retenção do usuário na plataforma).
* **Prioridade:** Média (Pode impactar taxas de conversão de vendas devido à lentidão no fluxo).

---

## 📷 Evidências e Anexos
> *(Insira uma captura de tela do carregamento da tela ou log do Network/Rede no DevTools indicando o tempo elevado de resposta)*
> 
> `![Evidência do Bug 005](./imagens/evidencia-bug-005.png)`
