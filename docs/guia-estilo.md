# Guia de estilo — Pastelaria Crumbly

> Versão provisória para a E3. A paleta e a tipografia podem ser revistas à medida que o projeto evoluir.

## Identidade visual

O site usa uma identidade acolhedora, inspirada numa pastelaria de bairro. Os tons de creme e papel claro formam os fundos; castanhos são usados no texto; laranja e dourado destacam a marca e os elementos de interação.

## Paleta de cores

| Cor | Código | Utilização atual |
|---|---|---|
| Creme | `#FFF8EB` | Cabeçalho, secções alternadas e fundos suaves |
| Papel | `#FFFDF8` | Fundo principal e cartões |
| Castanho | `#4A2B20` | Texto principal e rodapé |
| Castanho claro | `#795342` | Texto secundário |
| Laranja | `#C85B27` | Cor de destaque e detalhes |
| Laranja escuro | `#9E3F18` | Marca, botões, ligações ativas e foco |
| Dourado | `#E7A642` | Detalhes decorativos e foco no rodapé |
| Linha | `#EAD8C0` | Contornos e divisórias |

Os valores correspondem às variáveis definidas em [`../css/style.css`](../css/style.css).

## Tipografia

- **Texto corrido e títulos:** Georgia, com Times New Roman como alternativa serifada e a fonte padrão do sistema como último recurso.
- **Elementos de interface:** Arial, com uma fonte sans-serif do sistema como alternativa, usada na marca, nos botões, nos pequenos rótulos e nos títulos da tabela.
- **Hierarquia:** títulos principais são grandes e ajustam-se ao ecrã; os títulos de secção usam tamanhos intermédios; o texto corrido mantém espaçamento de linha confortável.

## Contraste e combinações de texto

Os rácios abaixo foram calculados a partir dos valores hexadecimais da paleta, segundo a fórmula de luminância relativa do WCAG. Para texto normal, o mínimo de referência é 4,5:1; para texto grande, 3:1.

| Cor do texto | Fundo | Rácio | Resultado |
|---|---|---:|---|
| Castanho `#4A2B20` | Papel `#FFFDF8` | 12,46:1 | Cumpre ambos os mínimos |
| Castanho `#4A2B20` | Creme `#FFF8EB` | 11,99:1 | Cumpre ambos os mínimos |
| Castanho claro `#795342` | Papel `#FFFDF8` | 6,60:1 | Cumpre ambos os mínimos |
| Castanho claro `#795342` | Creme `#FFF8EB` | 6,35:1 | Cumpre ambos os mínimos |
| Laranja escuro `#9E3F18` | Papel `#FFFDF8` | 6,50:1 | Cumpre ambos os mínimos |
| Laranja escuro `#9E3F18` | Creme `#FFF8EB` | 6,26:1 | Cumpre ambos os mínimos |
| Branco `#FFFFFF` | Laranja escuro `#9E3F18` | 6,61:1 | Cumpre ambos os mínimos |
| Branco `#FFFFFF` | Castanho `#4A2B20` | 12,67:1 | Cumpre ambos os mínimos |
| Creme `#FFF8EB` | Castanho `#4A2B20` | 11,99:1 | Cumpre ambos os mínimos |

O laranja `#C85B27`, o dourado `#E7A642` e a cor de linha `#EAD8C0` ficam reservados a detalhes, contornos ou decoração sobre fundos claros; não devem ser usados como texto nesses fundos. O dourado também é usado no contorno de foco sobre o rodapé castanho, com rácio de 5,99:1.

## Aplicação

Manter contraste entre texto e fundo, reservar as cores de destaque para ações e elementos importantes, e usar a mesma família tipográfica de forma consistente nas cinco páginas.
