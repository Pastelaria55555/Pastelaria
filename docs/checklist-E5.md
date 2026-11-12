# Checklist E5 — Design responsivo

- [x] Abordagem mobile-first: os estilos base começam em uma coluna e os layouts maiores são acrescentados nos breakpoints `600px`, `900px` e `1200px`.
- [x] Flexbox na navegação e grelha CSS na galeria de conteúdos.
- [x] As cinco páginas foram verificadas em viewports reais de 360 px e 1280 px sem conteúdo fora da largura disponível; capturas em `docs/responsivo/`.
- [x] Pelo menos duas imagens usam a classe `responsive-image`, que aplica `max-width: 100%` e `height: auto`.
- [x] Elementos interativos principais e controlos de seleção têm áreas de toque com pelo menos 24 × 24 px; navegação, botões e resumo usam 44 px de altura.
- [x] A tag Git `E5` foi criada anteriormente; esta atualização não cria commits nem altera a tag.

## Verificações

- Capturas: [evidências responsivas](./responsivo/README.md).
- Nas cinco páginas, em 360 px e 1280 px, `documentElement.scrollWidth` não excedeu a largura disponível. A verificação não encontrou elementos com conteúdo interno mais largo do que a caixa; as tabelas do menu também cabem sem scroll horizontal.
- HTML: submeter individualmente as cinco páginas ao Nu Html Checker; guardar os resultados oficiais, se a unidade curricular pedir evidências do validador nesta entrega.
- Interação: percorrer a navegação e o formulário por teclado e confirmar o foco visível.
