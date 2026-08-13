# Bancadas Modulares — catálogo interativo (configurador)

Demonstração de **catálogo digital interativo** para um produto **modular**: bancadas de
trabalho industriais. Em vez de uma lista estática, o cliente **monta a bancada** e o pedido
sai pelo WhatsApp já especificado.

🔗 **Demo ao vivo:** https://eduardoeug.github.io/workana/bancadas/

## O que a demo faz

- **Configurador** com as opções reais do produto: **8 comprimentos**, **3 alturas**,
  **3 profundidades**, **3 padrões de cor** e **5 acessórios** (prateleira superior, painel
  porta-ferramentas, gaveteiro, iluminação LED e rodízios).
- **Desenho que muda na hora**: a bancada é redesenhada em SVG a cada escolha — fica mais
  larga/alta, muda de cor e ganha os acessórios selecionados, com as **cotas** (comprimento,
  altura, profundidade) marcadas no desenho.
- **Modelos prontos** (Compacta / Padrão / Industrial) pra carregar uma configuração num clique.
- **Resumo do pedido** + **código da configuração** (ex.: `BM-200-090-070-AL-PSPF`).
- **Botão de WhatsApp** que abre a conversa **já preenchida** com toda a especificação
  escolhida — o vendedor recebe o pedido pronto, sem ficar perguntando medida por medida.
- Mobile-first (o link de catálogo é aberto no celular na maioria das vezes).

## Observação

Medidas, cores, acessórios e o número do WhatsApp são **exemplos** — na versão real entram a
tabela de produtos e o número do cliente. Dá pra incluir também preço por configuração.

## Tecnologia

HTML, CSS e JavaScript puro — sem build e sem dependências. O desenho da bancada é **SVG
gerado por código** (escala conforme as medidas escolhidas), então não precisa de foto de
cada combinação possível.
