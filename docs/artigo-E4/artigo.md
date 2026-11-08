# Modelo de caixa e layout numa página Web simples

## Tema

Aplicação do modelo de caixa, de layouts simples e de elementos HTML5 na interface da Pastelaria Crumbly.

## Questão orientadora

Como pode uma página Web de uma pastelaria organizar texto, imagens, tabelas e formulários de forma clara, consistente e utilizável apenas com HTML e CSS?

## Índice

1. Introdução
2. O modelo de caixa
3. Organização do layout
4. Elementos HTML5 com significado
5. Tabelas e formulários
6. Navegação por teclado
7. Conclusão
8. Referências

## 1. Introdução

Uma página Web é formada por elementos que ocupam espaço e se relacionam entre si. Na Pastelaria Crumbly, o objetivo da E4 é aplicar os conteúdos da sessão sobre modelo de caixa e layout a uma página que seja fácil de ler em computador e telemóvel.

## 2. O modelo de caixa

Cada elemento visível pode ser entendido como uma caixa formada por conteúdo, espaçamento interior, borda e margem exterior. No projeto, a regra `box-sizing: border-box` facilita o cálculo das larguras, porque o `padding` e a `border` ficam incluídos na largura definida. As classes de cartões, tabelas e campos do formulário usam `padding` para criar espaço interior, `border` para separar áreas e `margin` ou `gap` para separar elementos.

## 3. Organização do layout

O contentor principal limita a largura do conteúdo e centra as páginas. O cabeçalho e o rodapé usam flexbox para distribuir a marca e a navegação. As grelhas da página inicial, das duas colunas e do formulário organizam os elementos em linhas e colunas. Em ecrãs estreitos, uma regra `@media` transforma essas áreas numa coluna para evitar que o conteúdo fique apertado.

## 4. Elementos HTML5 com significado

Além de `header`, `nav`, `main`, `section`, `article` e `footer`, foram usados elementos com funções específicas. `figure` e `figcaption` associam uma imagem à sua legenda. `details` e `summary` apresentam uma nota que o utilizador pode abrir. `time` identifica anos e horas. `mark` chama a atenção para uma informação curta. Estes elementos ajudam a dar significado ao conteúdo sem recorrer a componentes complexos.

## 5. Tabelas e formulários

O menu usa tabelas com `caption`, cabeçalhos de coluna e cabeçalhos de linha. O formulário de contactos usa `label`, `input`, `select`, `textarea`, `fieldset` e `legend`. Os campos têm espaçamento e bordas consistentes com o resto do site. A validação simples é feita pelos atributos HTML nativos, como `required`, `type="email"` e `pattern`.

## 6. Navegação por teclado

As ligações e os controlos nativos podem ser alcançados com a tecla `Tab`. A regra `:focus-visible` acrescenta um contorno castanho visível, com espaço em redor, para indicar o elemento ativo. A ordem segue a ordem do HTML, começando no cabeçalho e terminando no rodapé.

## 7. Conclusão

O modelo de caixa permite controlar o espaço de cada componente. O layout com contentores, flexbox, grelhas e uma adaptação simples para ecrãs pequenos mantém as páginas organizadas. Os elementos HTML5 tornam o conteúdo mais claro e o foco visível melhora a utilização sem rato.

## 8. Referências

Data de acesso de todas as referências: **08-11-2026**.

1. Mozilla Developer Network. “CSS box model”. [https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Box_model](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Box_model)
2. Mozilla Developer Network. “Introduction to the CSS box model”. [https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Box_model/Introduction](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Box_model/Introduction)
3. Mozilla Developer Network. “CSS flexible box layout”. [https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Flexible_box_layout)
4. Mozilla Developer Network. “The article element”. [https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/article](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/article)
5. Mozilla Developer Network. “The details disclosure element”. [https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/details](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/details)
6. Mozilla Developer Network. “The time element”. [https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/time](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/time)
7. W3C Web Accessibility Initiative. “Understanding Focus Visible”. [https://www.w3.org/WAI/WCAG22/Understanding/focus-visible](https://www.w3.org/WAI/WCAG22/Understanding/focus-visible)
8. W3C. “Nu Html Checker”. [https://validator.w3.org/nu/](https://validator.w3.org/nu/)
