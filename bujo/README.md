# Rotina — app de Bullet Journal (demo navegável)

Protótipo interativo de um **app de rotina pessoal no método Bullet Journal** — feito para
mostrar o fluxo funcionando antes do desenvolvimento.

🔗 **Demo ao vivo:** https://eduardoeug.github.io/workana/bujo/

## O diferencial: o método, respeitado

A maioria dos apps chama de "bullet journal" uma lista de tarefas comum. Esta demo implementa
o que realmente define o método:

- **Registro rápido** com os significantes reais: `•` tarefa, `○` evento, `—` nota;
- **Migração** — o coração do BuJo: a tarefa não feita não some, ela é **migrada
  conscientemente** (`>`). Na demo, tocar numa tarefa alterna `aberta → concluída (×) →
  migrada (>)`;
- **Log diário, mensal e futuro** — inclusive o calendário do mês marcando os dias com registro;
- **Coleções** personalizadas (livros, metas, ideias) e **habit tracker** com marcação por dia
  e percentual da semana.

## Interativo de verdade

Dá para tocar nas tarefas, concluir, migrar, **criar registros novos** (escolhendo o
significante) e marcar hábitos — tudo respondendo na hora.

## Observação

Layout, cores e conteúdo são um ponto de partida; na versão real entram a identidade e as
preferências do cliente. No app final: **offline primeiro**, busca e tags, lembretes da revisão
diária/mensal e Android (React Native, para sair iOS do mesmo código se quiser depois).

## Tecnologia

HTML, CSS e JavaScript puro — sem build, sem dependências.
