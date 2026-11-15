# Relatório de auditoria inicial — E6

**Data dos resultados registados:** 15-11-2026
**Páginas observadas:** `index.html`, `menu.html` e `sobre.html`
**Estado:** Lighthouse e WAVE repetidos após as correções nas três páginas. WAVE apresenta 0 erros, 0 erros de contraste e 0 alertas; Lighthouse apresenta as pontuações abaixo em modo Mobile.

## Método e limites

As três páginas foram analisadas com Lighthouse no Chrome em `http://localhost:8000`, em modo **Mobile** (a pré-visualização do relatório mostra a viewport móvel), e com a extensão WAVE. As capturas de ambas as ferramentas foram feitas após as correções. Também foram observadas as árvores de acessibilidade e, com a inspeção do DOM no navegador, foram verificados título, número de H1, imagens, foco após `Tab` e largura do documento. Foi feita uma verificação local dos destinos relativos de ligações e folhas de estilo referidos nestas páginas.

Os valores abaixo foram transcritos das capturas fornecidas. Os contadores WAVE de Features, Structure e ARIA são apresentados como informação da ferramenta, não como erros. A WAVE indica que continua a ser necessário teste manual.

## Resultados Lighthouse comunicados

| Página | Desempenho | Acessibilidade | Boas práticas | SEO | Modo |
| --- | ---: | ---: | ---: | ---: | --- |
| `index.html` | 99 | 100 | 96 | 100 | Mobile |
| `menu.html` | 99 | 100 | 96 | 100 | Mobile |
| `sobre.html` | 99 | 100 | 96 | 100 | Mobile |

As capturas Lighthouse estão guardadas no repositório: [index](./evidencias/lighthouse-E6-index.png), [menu](./evidencias/lighthouse-E6-menu.png) e [sobre](./evidencias/lighthouse-E6-sobre.png).

## Resultados WAVE

| Página | Erros | Erros de contraste | Alertas | Features | Structure | ARIA | AIM Score |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| `index.html` | 0 | 0 | 0 | 6 | 12 | 9 | 10/10 |
| `menu.html` | 0 | 0 | 0 | 4 | 43 | 7 | 10/10 |
| `sobre.html` | 0 | 0 | 0 | 4 | 11 | 7 | 10/10 |

Capturas WAVE guardadas no repositório: [index](./evidencias/WAVE-E6-index.png), [menu](./evidencias/WAVE-E6-menu.png) e [sobre](./evidencias/WAVE-E6-sobre.png). As capturas Lighthouse também já estão guardadas: [index](./evidencias/lighthouse-E6-index.png), [menu](./evidencias/lighthouse-E6-menu.png) e [sobre](./evidencias/lighthouse-E6-sobre.png).

Na análise WAVE anterior, foram identificados: **“Redundant link”** para “Início”, porque a marca/logótipo e essa ligação da navegação apontavam ambos para `index.html`; e texto demasiado pequeno na badge **“Forno diário”** da página inicial. O padrão de ligação repetida existia no código das cinco páginas. A badge foi aumentada para `font-size: 0.8rem` em `css/bootstrap-custom.css`, e a ligação “Início” foi retirada da navegação nas cinco páginas, mantendo-se o logótipo como ligação para a página inicial. Nas novas capturas WAVE, as três páginas apresentam zero alertas.

## Observações complementares

| Página | Observações confirmadas nesta inspeção |
| --- | --- |
| `index.html` | Um H1; cinco imagens carregadas; todas têm `alt` (a imagem decorativa do logótipo tem `alt` vazio e está dentro de um elemento `aria-hidden`); numa observação anterior, o logótipo recebeu foco visível. A repetição atual do teste com `Tab` não foi conclusiva, pois o navegador de teste manteve o foco no `body`; sem overflow horizontal observado a 360 px e 1280 px. |
| `menu.html` | Um H1; duas imagens carregadas e com `alt`; duas tabelas expostas como tabelas, com legenda e cabeçalhos de coluna identificados; a observação anterior indicava foco no logótipo com `Tab`, mas não foi possível repetir conclusivamente a passagem completa agora; sem overflow horizontal observado a 360 px e 1280 px. |
| `sobre.html` | Um H1; três imagens carregadas e com `alt`; a observação anterior indicava foco no logótipo com `Tab`, mas não foi possível repetir conclusivamente a passagem completa agora; sem overflow horizontal observado a 360 px e 1280 px. |

Na verificação local, as páginas HTML, folhas de estilo e destinos internos observados existem. Isto confirma apenas a existência dos caminhos verificados; não é uma avaliação geral de qualidade ou acessibilidade.

## Problemas e plano de correção

| Problema / estado | Prioridade | Plano |
| --- | --- | --- |
| A ligação “Início” era assinalada como “Redundant link” e o texto “Forno diário” era assinalado como demasiado pequeno. | Corrigido e verificado no WAVE | A navegação foi simplificada nas cinco páginas e a badge aumentada para `0.8rem`. A nova análise WAVE mostra 0 alertas nas três páginas testadas. |
| A repetição atual do teste de teclado não foi conclusiva no navegador de teste. | Pendente de confirmação manual | No navegador do utilizador, percorrer cada página com `Tab` e `Shift+Tab`, confirmar o contorno visível, ativar ligações com `Enter` e testar o controlo `details` do menu com teclado. Registar o resultado após observação direta. |

## Próximos passos

1. Manter as capturas atuais de Lighthouse e WAVE como evidência das páginas corrigidas.
2. Completar a confirmação manual de teclado no navegador do utilizador; as ferramentas automáticas não substituem este teste.
