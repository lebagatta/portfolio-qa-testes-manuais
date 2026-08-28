# [BUG-022] Componente Radio Button com opção "Não" desabilitada para seleção do usuário

## 📌 Descrição Geral
Na página de botões de opção (`/radio-button`), sob a pergunta *"Você gosta do site?"*, a terceira opção de resposta (**"Não"**) encontra-se permanentemente desabilitada. O elemento não responde a cliques e não permite que o usuário registre uma avaliação negativa.

---

## 🛠️ Informações do Ambiente
* **Aplicação:** DemoQA
* **URL:** `https://demoqa.com/radio-button`
* **Navegador:** Microsoft Edge / Google Chrome

---

## 📋 Passos para Reproduzir
1. Acesse `https://demoqa.com/`.
2. Acesse a seção **Elements** e clique na opção **Radio Button** (`/radio-button`).
3. Tente clicar na opção **"Não"** (*No*).
4. Observe a ausência de resposta e a alteração da seleção.

---

## 🎯 Comportamento Esperado
* Todas as opções de resposta ("Sim", "Impressionante" e "Não") devem estar habilitadas e ser interativas, permitindo a seleção individual por parte do usuário.

---

## ❌ Comportamento Atual (Bug)
* O botão de rádio relativo à opção "Não" possui o atributo `disabled`, apresentando estado visual inativo e impedindo qualquer interação ou seleção.

---

## ⚡ Severidade e Prioridade
* **Severidade:** Média (Impedimento de registro de feedback/opção por parte do usuário).
* **Prioridade:** Média (Afeta a integridade da funcionalidade e a coleta de dados de pesquisa).

---

## 📷 Evidências e Anexos
*Evidência pendente de inclusão.*
