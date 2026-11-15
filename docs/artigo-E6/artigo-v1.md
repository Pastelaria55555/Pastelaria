# Bootstrap e auditoria inicial num sítio Web de pastelaria

**Entrega:** E6 — Bootstrap e auditoria inicial
**Versão:** 1 — 15-11-2026
**Estado:** primeira versão redigida; inclui resultados Lighthouse e WAVE após correções nas três páginas auditadas.

## Questão orientadora

Como pode o Bootstrap ajudar a organizar páginas responsivas sem substituir a identidade visual nem a verificação de acessibilidade do sítio?

## Índice

1. Introdução
2. O que é o Bootstrap
3. Grelha e componentes no projeto
4. Personalização e identidade visual
5. Auditoria inicial
6. Resultados preliminares e plano de correção
7. Conclusão provisória
8. Referências

## 1. Introdução

Um sítio Web deve apresentar o seu conteúdo de forma organizada em ecrãs de tamanhos diferentes. No projeto da Pastelaria Crumbly, as páginas já tinham uma folha de estilos própria. Nesta etapa foi introduzido o Bootstrap, uma framework CSS que disponibiliza classes para grelhas, tabelas, botões e outros elementos comuns. O objetivo não é refazer o sítio nem acrescentar funcionalidades fora do âmbito da entrega: é experimentar ferramentas de layout e componentes, mantendo o aspeto tradicional da pastelaria.

Esta versão explica a escolha do Bootstrap, a sua utilização nas páginas e os resultados de uma auditoria inicial. As capturas documentam as ferramentas e páginas analisadas; os resultados não substituem uma revisão manual de teclado e conteúdo.

## 2. O que é o Bootstrap

O Bootstrap é uma framework de CSS que fornece estilos e classes reutilizáveis. Em vez de escrever do início todas as regras de uma grelha ou de uma tabela, o autor pode aplicar classes documentadas e concentrar-se na estrutura e no conteúdo. A versão usada neste projeto é a **5.3.9**, carregada através da folha de estilos oficial por CDN. A versão fica indicada no README para que seja possível identificar a dependência usada.

A framework não decide sozinha se uma página é clara, acessível ou adequada ao tema. As classes aplicadas continuam a precisar de ser verificadas no contexto do sítio. Por exemplo, uma tabela pode receber estilos visuais do Bootstrap, mas ainda precisa de cabeçalhos que expliquem os dados. Do mesmo modo, uma ligação com aparência de botão deve continuar a levar a um destino coerente e a ser identificável por teclado.

## 3. Grelha e componentes no projeto

O sistema de grelha do Bootstrap usa contentores, linhas e colunas. As classes de coluna podem variar consoante a largura do ecrã, permitindo organizar o conteúdo em várias colunas quando há espaço e empilhá-lo em ecrãs pequenos. No projeto, a página inicial aplica a grelha à apresentação dos produtos e a página do menu organiza as suas secções com essa estrutura. A grelha é feita com classes HTML; não foi acrescentado código JavaScript para este efeito.

Foram integrados componentes simples: cartões para apresentar produtos, botões para as ligações em destaque, uma etiqueta informativa (badge), um alerta e tabelas para os produtos e preços. Estes elementos servem para dar consistência a conteúdos que já pertencem ao sítio. O menu continua a ser uma tabela de dados, com cabeçalhos, e não uma grelha improvisada de texto.

Uma framework pode alterar alguns detalhes visuais mesmo quando as páginas já têm CSS. Por isso, o projeto mantém as personalizações num ficheiro separado, `css/bootstrap-custom.css`. Nesse ficheiro são ajustadas cores, tipografia e alguns estilos de componentes. O objetivo é manter os tons creme, castanho e laranja e a letra serifada que caracteriza a pastelaria, sem modificar os ficheiros originais do Bootstrap. Separar os estilos também facilita perceber quais as regras que pertencem ao projeto.

## 4. Personalização e identidade visual

O nome e a apresentação do projeto apontam para uma pastelaria tradicional no Porto. A paleta quente e a tipografia serifada ajudam a manter essa identidade quando se usam classes da framework. As personalizações devem ser suficientes para integrar os componentes, mas não devem tornar o CSS difícil de explicar: cada regra acrescentada deve corresponder a uma alteração observável, como a cor dos botões ou o tipo de letra dos títulos.

É importante verificar as páginas em conjunto, porque uma regra global pode afetar títulos e texto fora do componente que motivou a mudança. A comparação deve incluir a página inicial, o menu e as restantes páginas que carregam o Bootstrap. Se uma alteração global piorar a leitura ou mudar demasiado o aspeto existente, deve ser ajustada no ficheiro de personalização, sem editar a framework.

## 5. Auditoria inicial

Uma auditoria inicial procura problemas que possam prejudicar a utilização das páginas. Para esta entrega, devem ser observadas três páginas com o Lighthouse e uma segunda ferramenta de acessibilidade, como axe ou WAVE, conforme o enunciado. O Lighthouse gera relatórios de auditoria no navegador, mas as pontuações não substituem a inspeção da página. As ferramentas de acessibilidade também ajudam a encontrar problemas, mas uma verificação automática não confirma todos os aspetos da experiência real.

Os testes devem ser feitos em condições registadas: indicar a página, a ferramenta, a data e, se possível, o modo de execução. É necessário distinguir avisos informativos de problemas que exigem correção. Cada problema deve ter uma descrição curta, a página onde aparece e uma ação prevista. Depois de corrigir, deve repetir-se o teste para confirmar o resultado; não se deve declarar uma melhoria sem uma nova observação.

As capturas Lighthouse atuais, em modo Mobile, mostram em cada página 99 em Desempenho, 100 em Acessibilidade, 96 em Boas práticas e 100 em SEO. As novas capturas WAVE mostram zero erros, zero erros de contraste e zero alertas nas três páginas. A ligação “Início” redundante foi removida da navegação nas cinco páginas, mantendo o logótipo como ligação à página inicial. O texto pequeno em “Forno diário” foi corrigido aumentando a badge para `0.8rem` em `css/bootstrap-custom.css`; a nova análise WAVE já não reporta alertas. Na inspeção complementar, as três páginas apresentaram um H1 e as imagens carregaram; não se observou overflow horizontal a 360 px nem a 1280 px. Uma observação anterior registou foco visível no logótipo, mas a tentativa atual de repetir o percurso completo com `Tab` não foi conclusiva no navegador de teste. No menu, as duas tabelas foram reconhecidas com legendas e cabeçalhos. O estado e o plano estão no [relatório E6](../relatorio-auditoria-E6.md).

## 6. Resultados e plano de correção

As capturas atuais de Lighthouse e WAVE estão guardadas em `docs/evidencias/` e registadas no relatório E6. Ambas as ferramentas foram repetidas após as correções. A confirmação manual completa de teclado continua pendente.

## 7. Conclusão

O Bootstrap acrescenta uma grelha e componentes que podem facilitar a organização do sítio, enquanto as personalizações mantêm a identidade visual da Pastelaria Crumbly. As pontuações Lighthouse e os resultados WAVE registam o estado das três páginas auditadas depois das correções. Como as verificações automáticas não cobrem toda a experiência, recomenda-se completar a avaliação com testes manuais de teclado e conteúdo.

## 8. Referências

Data de acesso: **15-11-2026**.

1. Bootstrap. “Introduction”. Documentação da versão 5.3. [https://getbootstrap.com/docs/5.3/getting-started/introduction/](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
2. Bootstrap. “Grid system”. [https://getbootstrap.com/docs/5.3/layout/grid/](https://getbootstrap.com/docs/5.3/layout/grid/)
3. Chrome for Developers. “Lighthouse overview”. [https://developer.chrome.com/docs/lighthouse/overview/](https://developer.chrome.com/docs/lighthouse/overview/)
4. W3C Web Accessibility Initiative. “Web Accessibility Evaluation Tools List”. [https://www.w3.org/WAI/test-evaluate/tools/list/](https://www.w3.org/WAI/test-evaluate/tools/list/)
5. W3C Web Accessibility Initiative. “Website Accessibility Conformance Evaluation Methodology (WCAG-EM)”. [https://www.w3.org/WAI/test-evaluate/conformance/wcag-em/](https://www.w3.org/WAI/test-evaluate/conformance/wcag-em/)
