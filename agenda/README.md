# Marca — agendamento online (demo em React)

Protótipo funcional de uma plataforma de **agendamento online** no estilo do
ageenda.com.br / Calendly, construído em **React**. Mostra os dois lados do produto:
o **cliente agendando** e o **profissional gerenciando** a agenda.

🔗 **Demo ao vivo:** https://eduardoeug.github.io/workana/agenda/

## O que a demo mostra

**Lado do cliente — fluxo de agendamento em 5 passos:**

- **Serviço** — catálogo com duração e preço (corte, barba, coloração, etc.).
- **Profissional** — só quem faz aquele serviço, com o **próximo horário livre** já calculado.
- **Data** — próximos 14 dias, respeitando os dias de trabalho de cada profissional.
- **Horário** — grade gerada a partir do expediente, **bloqueando almoço, horários já ocupados e horários que já passaram**.
- **Confirmação** — resumo, dados do cliente e tela de sucesso (com aceno a lembretes por e-mail/WhatsApp e integração de calendário).

**Lado do profissional — painel de gestão:**

- **Agenda do dia** por horário, com cliente, serviço, valor e cor por profissional.
- **Indicadores**: agendamentos do dia, **ocupação (%)**, **faturamento previsto** e clientes.
- **Filtro por profissional** e navegação pelos próximos 7 dias.
- **Cancelar** um agendamento (libera o horário na hora).
- Painéis de **serviços** (duração/preço) e **equipe & disponibilidade**.

> Agende na aba **Agendar** e veja o agendamento aparecer no **Painel** na mesma hora.

## Tecnologia

**React** (via htm, sem build) — componentes e estado com hooks; agendamentos salvos no
navegador (`localStorage`). No produto real, esse front em React conversa com um **backend
(Node.js ou .NET Core) + banco de dados**, arquitetura **multi-tenant** (cada negócio com
sua conta), autenticação, **lembretes automáticos** (e-mail/SMS/WhatsApp) e **integração
com Google Calendar / Outlook**.

> Protótipo demonstrativo, com dados fictícios. Não é o produto final.
