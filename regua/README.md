# Régua — cobrança de inadimplência no automático

Piloto de um sistema que **automatiza a cobrança de inadimplência** com uma
**régua de cobrança configurável**: puxa quem está devendo, decide a etapa certa de
cada um e dispara a mensagem na hora certa (WhatsApp, e-mail, SMS), sozinho — e mostra
a recuperação acontecendo em tempo real. Pensado **multi-cliente** (o mesmo sistema
atende vários shoppings, cada um com sua régua e seus dados isolados).

🔗 **Demo ao vivo:** https://eduardoeug.github.io/workana/regua/

## O que a demo mostra

- **Painel** — em aberto, recuperado no mês, **taxa de recuperação**, disparos de hoje;
  **valor em aberto por faixa de atraso** (aging), **inadimplentes por etapa** da régua e um
  feed da **régua em ação**.
- **Inadimplentes** — quem deve, quanto, há quantos dias, **em que etapa da régua está** e
  **qual a próxima ação** (data + canal). Busca, filtros (em cobrança / negociando / crítico /
  quitado) e ficha do lojista com **histórico de cobrança**.
- **Régua de cobrança** — o coração: etapas com **gatilho por dia** (D-3, no vencimento, D+3,
  D+8, D+15…), **canal** e **mensagem com variáveis** (`{nome}`, `{loja}`, `{valor}`, `{dias}`).
  Cada etapa liga/desliga e você pode **adicionar novas**.
- **Rodar a régua agora** — simula os disparos do dia: o sistema calcula quem cai em cada
  etapa, dispara pelo canal certo, registra o resultado (enviado → entregue → lido → respondeu)
  e alguns lojistas **negociam ou quitam** — saindo da régua e movendo os indicadores.
- **Disparos** — tudo que a régua enviou, com a mensagem já preenchida, filtrável por canal.
- **Integrações & canais** — origem dos dados (**ERP / planilha**) e canais (**WhatsApp API
  oficial**, e-mail, SMS, voz), além do seletor **multi-empresa** (Shopping Norte / Sul / Via).

> Troque de cliente no canto superior direito e veja tudo se recalcular. Na aba **Régua**,
> desligue uma etapa e veja o painel reagir. Toque em **Rodar a régua agora** para ver a
> automação disparar e a recuperação subir.

## Tecnologia

HTML, CSS e JavaScript puro — sem dependências nem build. Toda a lógica da régua (etapa de
cada inadimplente, próxima ação, disparos do dia, recuperação) roda no próprio front, com
dados fictícios.

> Protótipo demonstrativo. No produto real, o front conversa com um **backend
> (PHP/MySQL) + banco**, arquitetura **multi-tenant** (cada empresa com seus dados),
> **integração por API com o ERP** (ex.: Group Shopping) para puxar os inadimplentes,
> disparo pela **API oficial do WhatsApp Business** (+ e-mail/SMS), agendamento dos gatilhos,
> registro de cada tentativa e segurança/escala para volume alto.
