# Ana & Rafael — site de casamento + painel dos noivos + app (demo)

Demonstração de uma **plataforma multi-casamento**: vários casais, cada um com seu site de
mini destination wedding, seu painel e seus convidados — mais o mesmo código virando
**aplicativo mobile com Capacitor**.
o site dos convidados, o **painel de administração dos noivos** e o mesmo código virando
**aplicativo mobile com Capacitor**.

🔗 **Demo ao vivo:** https://eduardoeug.github.io/workana/casamento/

## As três partes (alternadas no topo)

**1. Site dos convidados** — mobile-first, porque o convidado abre pelo WhatsApp:
capa com contagem regressiva, programação dia a dia, hospedagem por faixa de preço e
distância, como chegar (aeroporto e transfer), o que fazer na região, traje, presentes
(Pix/lista) e **RSVP completo** (acompanhantes e restrição alimentar).

**2. Painel dos noivos** — o diferencial: confirmações em tempo real (confirmados,
aguardando, não vão, **total de pessoas para fechar com o buffet**), lista de convidados com
restrições consolidadas e edição do conteúdo do site pelos próprios noivos (mudou o horário
do transfer ou a diária do hotel, muda ali).

**3. App mobile (Capacitor)** — o mesmo código empacotado para Android e iOS, ganhando
notificação push (transfer, mudança de horário, contagem regressiva), funcionamento offline
(programação na praia sem sinal), ícone na tela do convidado e rota nativa.

## O que provar na demo

O **RSVP enviado no site aparece na hora no painel**, com os contadores recalculados — mostra
que é um sistema de verdade (site + API + banco + painel), não três telas desconectadas.

## Tecnologia

HTML, CSS e JavaScript puro nesta demo. No projeto real: front (React) + API + banco,
painel administrativo e **Capacitor** para gerar o app das lojas a partir do mesmo código —
começando pelo site (etapa 1) e evoluindo sem retrabalho.
