# Luxo On — Blueprint da Plataforma

Rascunho técnico interativo de uma plataforma concierge de beleza, mostrando como a
solução seria estruturada com **Softr + Airtable + Make + Stripe Connect + WhatsApp**.

🔗 **Demo ao vivo:** https://eduardoeug.github.io/workana/luxo-on/

## O que a demo mostra

- **Painel de parâmetros** — comissão, taxa fixa, valores de deslocamento e os critérios
  dos níveis (Parceira / Verificada / Premium) totalmente configuráveis. Nada chumbado no código.
- **Simulação do atendimento** — escolha serviço, zona e local e veja o sistema:
  - encontrar e ranquear as profissionais (nível → equilíbrio de carga → proximidade);
  - calcular a taxa de deslocamento pela média das 3 elegíveis mais próximas;
  - montar o split de pagamento (Stripe Connect) entre Luxo On e profissional, com a
    comissão incidindo só sobre o serviço (nunca sobre o deslocamento).
- **Modelo de dados (Airtable)** — tabelas, relações e campos calculados.
- **Níveis das profissionais** — recalculados ao vivo conforme os parâmetros.

## Tecnologia

HTML, CSS e JavaScript puro — sem dependências nem build.

> Protótipo demonstrativo, com dados fictícios. Não é o produto final.
