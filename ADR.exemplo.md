# 0001. Usar PostgreSQL como banco de dados principal

* **Status:** Aceito
* **Data:** 2026-09-11

## Contexto
Precisamos escolher um sistema de gerenciamento de banco de dados relacional para o novo microsserviço de cadastro de usuários.
O sistema precisa garantir forte consistência (ACID) para dados cadastrais e transacionais, além de possuir bom suporte na comunidade e facilidade de integração com a stack atual (Node.js/TypeScript).

## Decisão
Vamos adotar o **PostgreSQL** como o banco de dados relacional oficial do projeto.

## Alternativas Consideradas
* **MySQL:** Boa alternativa, mas a equipe possui mais familiaridade com recursos avançados do PostgreSQL (como tipos JSON nativos).
* **MongoDB:** Rejeitado por não garantir forte consistência transacional nativa (ACID por padrão) exigida pelo modelo de negócios atual.

## Consequências
* **Positivas:**
  * Garantia de integridade e consistência dos dados.
  * Facilidade para consultas complexas e relatórios.
* **Negativas:**
  * Maior complexidade de gerenciamento de infraestrutura em comparação a soluções gerenciadas mais simples.
  * Necessidade de planejar estratégias de escalabilidade horizontal no futuro.
