# Projeto Fictício - Backend 03

## 2. Achou! — Marketplace de E-commerce

**Contexto:** marketplace que conecta pequenos vendedores a compradores, com catálogo,
carrinho, pagamento e avaliação de vendedores.

**Escopo:** catálogo de produtos, busca, carrinho/checkout, integração com pagamento,
painel do vendedor.

**Restrição especial:** tráfego extremamente sazonal — picos de 20x o normal em datas
promocionais (ex: Black Friday), o resto do ano é tráfego baixo e estável.

**SLA desejado:** 99.5% de disponibilidade no dia a dia, mas zero tolerância a queda
durante campanhas promocionais.

**Stack/infra sugerida:** arquitetura que escale horizontalmente sob demanda (bom
candidato pra discutir serverless/auto-scaling); cache agressivo no catálogo/busca.

**Pico de uso:** extremamente concentrado em datas específicas — decisão de capacidade é
o desafio central desse projeto.

---
