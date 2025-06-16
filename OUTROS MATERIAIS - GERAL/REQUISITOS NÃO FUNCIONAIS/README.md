# Requisitos Não Funcionais

Esta seção descreve os requisitos de qualidade e restrições que o sistema deve atender. No Quadro 3, os Requisitos Não Funcionais estão numerados e classificados por categorias, com critérios claros de avaliação, garantindo que sejam objetivos, testáveis e alinhados aos objetivos do projeto.

### Quadro 3 - Requisitos não funcionais do sistema

| **Código** | **Categoria** | **Requisito Não Funcional** |
| --- | --- | --- |
| RNF01 | Acessibilidade | O sistema deve estar em conformidade com o nível *AA* das diretrizes de acessibilidade *WCAG 2.1*. |
| RNF02 | Desempenho | O tempo de resposta das funcionalidades de acessibilidade não deve ultrapassar 2 segundos após a interação do usuário. |
| RNF03 | Compatibilidade | O sistema deve ser compatível com os navegadores mais utilizados (*Google Chrome*, *Mozilla Firefox*, *Microsoft Edge*, *Safari*). |
| RNF04 | Portabilidade e Reutilização | O sistema deve garantir a persistência das preferências do usuário localmente (*cookies*/*local storage*) e/ou via nuvem (se login estiver disponível). |
| RNF05 | Disponibilidade | O sistema deve ter disponibilidade mínima de 99,5% mensal, considerando atualizações e manutenções planejadas. |
| RNF06 | Segurança | O sistema deve garantir segurança na autenticação do administrador por meio de criptografia de dados e, preferencialmente, autenticação de dois fatores. |
| RNF07 | Escalabilidade | A aplicação deve ser escalável para atender simultaneamente a múltiplos websites clientes utilizando o mesmo pacote de acessibilidade. |
| RNF08 | Internacionalização | O sistema deve ter suporte multilíngue, permitindo a tradução da interface e conteúdos auxiliares. |
| RNF09 | Usabilidade | O design da interface deve seguir princípios de usabilidade e acessibilidade, facilitando a navegação com teclado e leitores de tela. |