# [BUG-015] Quebra de layout e exibição de espaços em branco na grade de produtos

## 📌 Descrição Geral
Ao navegar pela página do catálogo completo de produtos (`/products`), a grade (*grid*) de exibição dos itens apresenta falhas de alinhamento e quebra de fluxo CSS. Embora a estrutura seja projetada para exibir 3 produtos por linha, surgem lacunas e espaços vazios no catálogo (com até 2 posições em branco por linha), desorganizando a disposição visual da vitrine.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** Automation Exercise
* **URL:** `https://automationexercise.com/products`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://automationexercise.com/`.
2. No menu superior, clique em **Products** (`/products`).
3. Role a página para baixo observando a distribuição dos cards de produtos.
4. Note a presença de lacunas/espaços vazios entre os cards nas linhas intermediárias da listagem.

---

## 🎯 Comportamento Esperado
* A vitrine de produtos deve manter uma distribuição uniforme e simétrica em formato de grade (3 colunas por linha), sem lacunas ou quebras de alinhamento no fluxo de produtos.

---

## ❌ Comportamento Atual (Bug)
* O layout da grade é interrompido por falhas de renderização CSS, deixando espaços em branco (lacunas) na vitrine de produtos e empurrando os itens seguintes para linhas inferiores.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Baixa (Não impede a navegação ou compra, mas degrada a interface do usuário).
* **Prioridade:** Média (Impacta a apresentação estestética, o acabamento do e-commerce e a experiência visual/UI).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
