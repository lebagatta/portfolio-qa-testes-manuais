# [BUG-025] Inconsistência de regra de negócio e interatividade no arraste do elemento inaceitável (Droppable)

## 📌 Descrição Geral
Na seção de interações (**Interactions** $\rightarrow$ **Droppable**), dentro da aba **Acceptable**, o elemento de teste denominado **"Not Acceptable"** não apresenta a restrição correta de comportamento ao ser arrastado para a área de destino (*Drop here*), mantendo o mesmo padrão de aceitação ou comportamento do elemento **"Acceptable"**.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** DemoQA
* **URL:** `https://demoqa.com/droppable`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://demoqa.com/droppable`.
2. Clique na aba **Acceptable**.
3. Arraste o bloco **"Acceptable"** para dentro da caixa *"Drop here"* e observe a reação do sistema.
4. Recarregue ou resete a tela e tente arrastar o bloco **"Not Acceptable"** para a mesma caixa *"Drop here"*.
5. Observe o comportamento e a falta de diferenciação na regra de rejeição do elemento.

---

## 🎯 Comportamento Esperado
* O container de destino deve rejeitar a soltura (*drop*) do bloco "Not Acceptable", não alterando seu estado/cor visual (ou retornando o bloco à posição de origem), sinalizando claramente ao usuário que aquele elemento não é permitido na área.

---

## ❌ Comportamento Atual (Bug)
* O sistema trata o elemento inaceitável com a mesma lógica do elemento permitido, sem aplicar o bloqueio visual ou a restrição de evento esperada para a regra de *Drag and Drop*.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Inconsistência de validação de regras em componentes interativos).
* **Prioridade:** Média (Interfere no entendimento e no fluxo de uso de componentes dinâmicos de arrastar e soltar).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
