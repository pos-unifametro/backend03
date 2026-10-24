# Projeto Fictício — Backend 03

## 1. PulsePay — Pagamentos Instantâneos

**Contexto:** fintech que processa transferências instantâneas entre contas de usuários
finais e pequenos comerciantes, similar a um PIX/carteira digital.

**Escopo:** cadastro/KYC básico de usuários, transferência entre contas, extrato,
notificação em tempo real de transação recebida.

**Restrição especial:** dados financeiros e pessoais devem permanecer em território
nacional (residência de dados) e toda transação precisa ser auditável (trilha imutável).

**SLA desejado:** 99.95% de disponibilidade; transação deve confirmar em até 2 segundos.

**Stack/infra sugerida:** arquitetura orientada a eventos, banco relacional para saldo/
transações + fila de mensagens; observabilidade forte é obrigatória (qualquer falha
silenciosa é inaceitável em pagamento).

**Pico de uso:** picos previsíveis (dias de pagamento de salário, datas comerciais).

---
