# Evidências de design responsivo — E5

As capturas documentam as cinco páginas em viewport real de telemóvel (360 px) e computador (1280 px).

| Página | Captura a 360 px | Captura a 1280 px |
|---|---|---|
| Início | `inicio-360.png` | `inicio-1280.png` |
| Menu | `menu-360.png` | `menu-1280.png` |
| Sobre nós | `sobre-360.png` | `sobre-1280.png` |
| Contactos | `contactos-360.png` | `contactos-1280.png` |
| Acessibilidade | `acessibilidade-360.png` | `acessibilidade-1280.png` |

As dez capturas foram geradas depois dos ajustes em páginas de teste com viewport real de 360 px e 1280 px. Nas cinco páginas, `documentElement.scrollWidth` não excedeu a largura disponível e não foram encontrados elementos com conteúdo interno mais largo do que a respetiva caixa. As tabelas do menu também cabem sem deslocamento horizontal interno.

Nota: nas capturas móveis, a imagem tem 345 px de largura porque o Chromium guarda a área de conteúdo sem os 15 px da barra vertical; o viewport de teste foi configurado para 360 px.
