# Vows — plataforma de sites de casamento (demo)

Demonstração de uma **plataforma multi-casamento**: vários casais, cada um com o seu site de
mini destination wedding, o seu painel e os seus convidados — mais o mesmo código virando
**aplicativo mobile com Capacitor**.

🔗 **Demo ao vivo:** https://eduardoeug.github.io/workana/casamento/

## Por que multi-casamento

Um site feito para um único casamento morre depois da festa. A mesma base atendendo **vários
casamentos** vira produto: cada casal entra com seu endereço (`vows.com.br/ana-e-rafael`), sua
identidade visual, sua programação e seus convidados — e **os dados de um casal nunca enxergam
os do outro**.

## As quatro visões (alternadas no topo)

**1. Site do casal** — mobile-first, porque o convidado abre pelo WhatsApp: capa com contagem
regressiva, programação dia a dia, hospedagem por faixa de preço e distância, como chegar
(aeroporto e transfer), o que fazer na região, traje, presentes e **RSVP completo**
(acompanhantes e restrição alimentar).

**2. Painel do casal** — confirmações em tempo real (confirmados, aguardando, não vão e
**total de pessoas para fechar com o buffet**), lista de convidados com restrições
consolidadas e edição do próprio site pelo casal.

**3. Plataforma** — visão de quem opera: todos os casamentos, convidados confirmados no total,
plano de cada casal e receita recorrente.

**4. App mobile (Capacitor)** — o mesmo código empacotado para Android e iOS, com notificação
push (transfer, mudança de horário, contagem regressiva), funcionamento offline e rota nativa.
Como a base é multi-casamento, **um app só** atende todos os casais.

## O que provar na demo

- **Trocar de casamento** no seletor muda o site inteiro: nomes, endereço, paleta, programação,
  hospedagem e lista de convidados.
- O **RSVP enviado no site aparece na hora** no painel daquele casal, com os contadores
  recalculados — e **não aparece** no painel dos outros (isolamento de dados).

## Tecnologia

HTML, CSS e JavaScript puro nesta demo. No projeto real: front (React) + API + banco com
arquitetura **multi-tenant**, painel administrativo e **Capacitor** para gerar o app das lojas
a partir do mesmo código — começando pelo site (etapa 1) e evoluindo sem retrabalho.
