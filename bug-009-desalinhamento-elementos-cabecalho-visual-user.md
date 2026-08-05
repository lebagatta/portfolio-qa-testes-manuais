# [BUG-009] Desalinhamento e quebra de layout nos botões do cabeçalho

## 📌 Descrição Geral
Ao navegar na aplicação com o perfil de teste visual, os elementos principais do cabeçalho superior (o menu hambúrguer de 3 traços no canto esquerdo e o ícone do carrinho de compras no canto direito) apresentam desalinhamento severo, deslocando-se para o centro da tela fora do padrão estético e da estrutura esperada da interface.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** SauceDemo (Swag Labs)
* **URL:** `https://www.saucedemo.com/inventory.html`
* **Navegador:** Microsoft Edge / Google Chrome
* **Perfil do Usuário Logado:** `visual_user`

---

## 📋 Passos para Reproduzir
1. Acesse `https://www.saucedemo.com/`.
2. Realize o login com o usuário `visual_user` e a senha `secret_sauce`.
3. Na página de vitrine (`/inventory.html`), observe o posicionamento dos ícones do topo da página (menu lateral e carrinho).

---

## 🎯 Comportamento Esperado
* Os ícones do menu lateral (esquerda) e do carrinho de compras (direita) devem permanecer fixos e alinhados às extremidades do cabeçalho, mantendo o padrão visual e a usabilidade.

---

## ❌ Comportamento Atual (Bug)
* Os botões do menu e do carrinho perdem o alinhamento relativo das margens e são renderizados deslocados para o meio da tela, sobrepondo áreas de conteúdo e quebrando o layout da aplicação.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Baixa (Não impede a execução das funcionalidades, mas degrada a experiência do usuário).
* **Prioridade:** Média (Impacta a apresentação visual e o acabamento profissional do produto).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
