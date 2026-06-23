# Bolso — controle financeiro pessoal

Protótipo mobile de um app de finanças pessoais: registra entradas e saídas, mostra o
saldo e revela para onde vai o dinheiro, com metas e alerta de estouro.

🔗 **Demo ao vivo:** https://eduardoeug.github.io/workana/financas/

## O que a demo mostra

- **Saldo total** no topo, com entradas e saídas do mês.
- **Gastos por categoria** num gráfico de rosca — cada setor é tocável e o maior gasto fica em destaque.
- **Drill-in**: toque numa categoria para ver o total e todas as transações dela.
- **Metas do mês** (total e por categoria) com **alerta quando o gasto estoura** o limite.
- **Lançamento manual** de transações (botão +), recalculando saldo, gráfico e metas ao vivo.
- Dados salvos localmente no navegador (`localStorage`).

## Tecnologia

HTML, CSS e JavaScript puro — sem dependências nem build. Pensado para a tela do celular.

> Protótipo demonstrativo, com dados fictícios. A versão final cobre Android e iOS (base única),
> contas de usuário e notificações; a conexão automática com o banco (Open Finance) é uma
> evolução opcional.
