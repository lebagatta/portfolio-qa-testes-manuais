Markdown
# 🧪 Portfólio de Garantia de Qualidade (QA) - Testes Manuais & Bug Reports

Profissional em transição para QA, com experiência prática em testes funcionais, exploratórios, validação de regras de negócio e documentação de defeitos. Este portfólio apresenta cenários reais de teste executados em aplicações web, incluindo identificação, reprodução, análise e documentação de bugs.

Este repositório reúne a documentação de testes manuais, testes exploratórios e relatórios de bugs identificados em diversas aplicações web e plataformas de e-commerce.

O objetivo é demonstrar a aplicação prática de análise de requisitos, mapeamento de cenários, testes cross-browser e reportes técnicos detalhados de falhas de software.

---

## 🛠️ Ferramentas e Tecnologias Utilizadas
* **Gerenciamento de Testes & Documentação:** Markdown, GitHub
* **Navegadores Utilizados (Cross-Browser):** Microsoft Edge, Google Chrome
* **Técnicas Aplicadas:** Testes Exploratórios, Validação de Regras de Negócio, Reporte de Bugs

---

## 📂 Estrutura do Repositório

├── testes-manuais/
│   ├── bug-001-filtro-ordem-alfabetica.md
│   ├── bug-002-falha-adicionar-produtos-carrinho.md
│   ├── bug-003-falha-nos-filtros-de-ordenacao.md
│   ├── bug-004-botao-remove-inoperante-na-vitrine.md
│   ├── bug-005-lentidao-e-latencia-no-carregamento.md
│   ├── bug-006-falha-adicao-e-remocao-vitrine-error-user.md
│   ├── bug-007-bloqueio-finalizacao-compra-checkout.md
│   ├── bug-008-excecao-alerta-falha-filtro-ordenacao.md
│   ├── bug-009-desalinhamento-elementos-cabecalho-visual-user.md
│   ├── bug-010-bloqueio-de-acesso-usuario-locked-out.md
│   ├── bug-011-imagens-duplicadas-vitrine-problem-user.md
│   ├── bug-012-sobrescrita-campo-sobrenome-checkout.md
│   └── bug-013-aceitacao-quantidade-negativa-produto.md
└── README.md

🐛 Relatórios de Bugs Registrados
🛍️ Aplicação: SauceDemo (Swag Labs)
[BUG-001] Filtro de ordenação alfabética (A-Z e Z-A) não respeita a ordem dos produtos: Ao selecionar os critérios de ordenação por nome, a listagem de produtos permanece de forma aleatória no navegador Microsoft Edge. (Ver detalhamento do Bug)

[BUG-002] Botão "Add to cart" inoperante em produtos específicos da vitrine: Ao tentar adicionar todos os itens ao carrinho com o perfil de teste, 3 produtos do catálogo não reagem ao clique do usuário. (Ver detalhamento do Bug)

[BUG-003] Inoperância total dos filtros de ordenação de produtos (Nome e Preço): No perfil problem_user, o seletor de ordenação não altera a disposição da vitrine ao escolher filtros por ordem alfabética ou por faixa de preço. (Ver detalhamento do Bug)

[BUG-004] Botão "Remove" inoperante na página de vitrine após adicionar produto: No perfil problem_user, o botão "Remove" na vitrine de produtos não responde ao clique para desfaçar a adição, obrigando a navegação até a tela de carrinho para excluir o item. (Ver detalhamento do Bug)

* **[BUG-005] Alta latência e gargalo de desempenho no carregamento e navegação:** No perfil `performance_glitch_user`, a aplicação apresenta atrasos severos no tempo de resposta durante o login e carregamento da vitrine, comprometendo a fluidez e a usabilidade. [(Ver detalhamento do Bug)](./testes-manuais/bug-005-lentidao-e-latencia-no-carregamento.md)

* **[BUG-006] Inoperância dos botões de Adição e Remoção de produtos na vitrine:** No perfil `error_user`, determinados produtos não permitem a adição ao carrinho e o botão "Remove" fica inoperante na vitrine, exigindo exclusão manual na tela do carrinho. [(Ver detalhamento do Bug)](./testes-manuais/bug-006-falha-adicao-e-remocao-vitrine-error-user.md)

* **[BUG-007] Impossibilidade de finalizar a compra (Botão "Finish" inoperante no Checkout):** No perfil `error_user`, a aplicação trava na etapa de resumo do pedido (`Overview`), pois o botão "Finish" não responde aos cliques, impedindo a conclusão do pedido. [(Ver detalhamento do Bug)](./testes-manuais/bug-007-bloqueio-finalizacao-compra-checkout.md)

* **[BUG-008] Exceção de sistema e mensagem de erro ao acionar filtro de ordenação:** No perfil `error_user`, ao selecionar qualquer opção no filtro de ordenação da vitrine, a aplicação dispara o alerta `"Sorting is broken! This error has been reported to Backtrace."` e impede a reordenação dos produtos. [(Ver detalhamento do Bug)](./testes-manuais/bug-008-excecao-alerta-falha-filtro-ordenacao.md)

* **[BUG-009] Desalinhamento e quebra de layout nos botões do cabeçalho:** No perfil `visual_user`, os ícones do menu lateral e do carrinho de compras perdem o alinhamento das margens e são renderizados deslocados em direção ao centro da tela, prejudicando a interface visual. [(Ver detalhamento do Bug)](./testes-manuais/bug-009-desalinhamento-elementos-cabecalho-visual-user.md)

* * **[BUG-010] Falha de autenticação e bloqueio de acesso no login (locked_out_user):** Ao tentar autenticar com a conta `locked_out_user`, a aplicação impede o acesso, exibindo alerta de conta bloqueada e retendo o usuário na tela de login. [(Ver detalhamento do Bug)](./testes-manuais/bug-010-bloqueio-de-acesso-usuario-locked-out.md)

* **[BUG-011] Renderização incorreta e duplicada das imagens de produtos na vitrine:** No perfil `problem_user`, todas as capas de produtos na vitrine carregam a mesma foto padrão de erro, omitindo as imagens reais do catálogo. [(Ver detalhamento do Bug)](./testes-manuais/bug-011-imagens-duplicadas-vitrine-problem-user.md)    

* **[BUG-012] Apagamento automático e falha na retenção de texto no campo "Last Name" do Checkout:** No perfil `problem_user`, o campo de sobrenome apaga automaticamente qualquer caractere digitado pelo usuário, impedindo o avanço do checkout devido à validação de campo obrigatório. [(Ver detalhamento do Bug)](./testes-manuais/bug-012-sobrescrita-campo-sobrenome-checkout.md)

* **[BUG-013] Permitida a adição de produtos com quantidade zero ou negativa ao carrinho:** No site Automation Exercise, o campo de quantidade da página de detalhes do produto permite valores inferiores a 1, adicionando itens com quantidades inválidas ao carrinho e afetando o cálculo do pedido. [(Ver detalhamento do Bug)](./testes-manuais/bug-013-aceitacao-quantidade-negativa-produto.md)
  
👤 Autor
Dr. Leandro Bagatta

GitHub
