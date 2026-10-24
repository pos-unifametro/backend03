# Projeto Fictício - Backend 03 

## 3. RotaCerta — Logística e Rastreamento de Entregas

**Contexto:** sistema que rastreia entregas em tempo real para uma transportadora de
médio porte, com atualização de posição via app dos entregadores.

**Escopo:** cadastro de entregas, rastreamento em tempo real, notificação de status ao
cliente final, painel operacional para a transportadora.

**Restrição especial:** entregadores usam conexão de internet instável (áreas rurais/
periferia) — o sistema precisa tolerar dados atrasados ou fora de ordem.

**SLA desejado:** 99% de disponibilidade; atualização de posição pode atrasar até 2
minutos sem ser considerado falha.

**Stack/infra sugerida:** boa oportunidade pra discutir filas/mensageria para lidar com
dados assíncronos e fora de ordem; monitoramento de dispositivos remotos.

**Pico de uso:** picos diários previsíveis (períodos de entrega concentrados, ex.
fim de tarde).

---

