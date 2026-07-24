# 🧪 Projeto de Garantia de Qualidade (QA) - SauceDemo

Este repositório contém a documentação completa dos testes manuais e exploratory realizados na aplicação e-commerce **[SauceDemo (Swag Labs)](https://www.saucedemo.com/)**.

O objetivo deste projeto é demonstrar a aplicação prática de técnicas de análise de requisitos, criação de casos de teste, identificação de falhas de usabilidade/cross-browser e documentação profissional de bugs.

---

## 🛠️ Ferramentas e Tecnologias Utilizadas
* **Gerenciamento de Testes & Documentação:** Markdown, GitHub
* **Navegadores Utilizados (Cross-Browser):** Microsoft Edge, Google Chrome
* **Técnicas Aplicadas:** Testes Exploratórios, Validação de Regras de Negócio, Reporte de Bugs

---

## 📂 Estrutura do Repositório

```text
├── testes-manuais/
│   └── BUG-001-filtro-ordem-alfabetica.md
└── README.md

🐛 Principais Bugs Identificados
[BUG-001] Filtro de ordenação alfabética (A-Z e Z-A) não respeita a ordem dos produtos: Ao selecionar os critérios de ordenação por nome, a listagem de produtos permanece de forma aleatória no navegador Microsoft Edge. (Ver detalhamento do Bug)

👤 Autor
Dr. Leandro Bagatta

GitHub

## 🐛 Principais Bugs Identificados

* **[BUG-001] Filtro de ordenação alfabética (A-Z e Z-A) não respeita a ordem dos produtos:** [(Ver detalhamento do Bug)](./testes-manuais/BUG-001-filtro-ordem-alfabetica.md)
* **[BUG-002] Botão "Add to cart" inoperante em produtos específicos da vitrine:** Ao tentar adicionar todos os itens ao carrinho, 3 produtos do catálogo não reagem ao clique no navegador Microsoft Edge. [(Ver detalhamento do Bug)](./testes-manuais/BUG-002-falha-adicionar-produtos-carrinho.md)
