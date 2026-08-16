# Blog + Portal Admin — demonstração navegável

Demo de um **blog corporativo** com a estrutura enviada pelo cliente (destaques, filtro por
categoria, busca, grid com paginação e newsletter) **mais o portal administrativo** que permite
à equipe publicar sozinha, sem depender de programador.

🔗 **Demo ao vivo:** https://eduardoeug.github.io/workana/bibllo/

## As duas visões (seletor no topo)

**1. Blog (leitor)**
- Seção de destaques: 1 card principal + 3 secundários;
- **Filtro por categoria** funcionando (Vendas, Gestão, Finanças, Pessoas, Marketing, Carreira,
  Tendências);
- **Busca de artigos** em tempo real (título, resumo e categoria);
- Grid de artigos com **paginação** e contagem de resultados;
- Página interna do artigo (categoria, título, autor, data, corpo);
- Bloco de newsletter com captura de e-mail;
- Header e footer no padrão do produto.

**2. Portal admin**
- **Artigos**: lista com status, categoria, autor e destaque; edição de qualquer artigo;
- **Novo artigo**: título, categoria, autor, resumo, conteúdo, status (publicado/rascunho) e
  destaque, com **campos de SEO e prévia de como aparece no Google**;
- **Destaque em um clique**: alternar entre principal (card grande), secundário e nenhum;
- **Categorias**: criar e remover — são exatamente os filtros da home;
- **Autores**: contagem de artigos por autor (base da página de autor);
- **Newsletter**: inscritos e exportação.

## O que a demo prova

- Publicar um artigo no admin marcando-o como **destaque** troca o card grande da home **na hora**;
- Uma inscrição feita no bloco de newsletter do blog **aparece imediatamente** na lista do admin.

Ou seja: é um sistema (site + painel), não telas soltas.

## Observação

Conteúdo, cores e marca são ilustrativos — na entrega real entram a identidade do cliente e o
conteúdo dele. Nesta demo o filtro e a busca rodam no navegador; no projeto real são feitos no
servidor, para escalar com centenas de artigos e dar **URL própria e indexável a cada categoria**.

## Tecnologia

HTML, CSS e JavaScript puro — sem build, sem dependências.
