# Teste de teclado — E4

## Método

1. Abrir cada página no navegador.
2. Clicar na barra de endereço e carregar em `Tab` repetidamente.
3. Confirmar que a ordem passa pelo logótipo, navegação, ligações do conteúdo, formulários e rodapé.
4. Confirmar que cada elemento ativo apresenta um contorno visível.
5. Usar `Enter` para abrir ligações e `Espaço` para abrir/fechar a nota de preços em `menu.html`.

## Resultado esperado

As ligações e controlos devem ser alcançáveis sem rato. O foco deve permanecer visível e seguir uma ordem lógica de leitura.

## Resultado registado

O CSS aplica `:focus-visible` a elementos interativos, com contorno de 3 px e afastamento de 3 px. A navegação usa ligações HTML normais e o formulário usa controlos HTML nativos, pelo que o percurso pode ser feito com `Tab`, `Shift+Tab`, `Enter` e as teclas próprias de cada controlo.

Data do registo: 08-11-2026.

Captura do teste: [`e4-teclado-menu.png`](./evidencias/e4-teclado-menu.png).
