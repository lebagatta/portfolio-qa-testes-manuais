# [BUG-024] Falha de renderização e sobreposição visual (rabisco) no item Widgets do menu lateral

## 📌 Descrição Geral
Ao navegar pelas seções do site, o item de menu **Widgets** na barra de navegação lateral esquerda apresenta uma falha crítica de renderização CSS. O texto e os elementos visuais aparecem sobrepostos e rabiscados, tornando o rótulo do menu completamente ilegível para o usuário.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** DemoQA
* **URL:** `https://demoqa.com/widgets` (ou em qualquer navegação com o menu lateral ativo)
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://demoqa.com/`.
2. Clique em qualquer seção para abrir a navegação lateral (ex: *Elements* ou *Widgets*).
3. Observe a lista de opções no menu sanfona (*accordion*) localizado à esquerda.
4. Analise a renderização visual do cabeçalho da categoria **Widgets**.

---

## 🎯 Comportamento Esperado
* O item de menu "Widgets" deve ser exibido com tipografia clara, alinhamento correto, espaçamento adequado e sem sobreposição de caracteres ou estilos CSS quebrados.

---

## ❌ Comportamento Atual (Bug)
* O texto da categoria "Widgets" e seus elementos visuais são renderizados de forma distorcida e sobreposta, criando um efeito de "rabisco" que impede a leitura limpa do componente.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Baixa/Média (Bug de UI/UX que não impede a navegação via clique, mas afeta a acessibilidade e estética do produto).
* **Prioridade:** Média (Interfere na percepção de qualidade e usabilidade visual da plataforma).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
