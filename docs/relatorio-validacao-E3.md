# Relatório de validação E3

## Folha de estilos externa

Verificação realizada em 25-10-2026 por inspeção dos cinco ficheiros HTML do projeto.

| Página | Folha de estilos ligada |
|---|---|
| [Início](../index.html) | `css/style.css` |
| [Menu](../menu.html) | `css/style.css` |
| [Sobre nós](../sobre.html) | `css/style.css` |
| [Contactos](../contactos.html) | `css/style.css` |
| [Acessibilidade](../acessibilidade.html) | `css/style.css` |

## Estilos em linha

Foi feita uma pesquisa nos cinco ficheiros HTML por elementos `<style>` e atributos `style`. Não foram encontrados estilos CSS em linha. Assim, todos os estilos das páginas são definidos na folha externa `css/style.css`.

## Resultado

**Ponto 1 da E3: cumprido.** Esta verificação confirma a ligação da folha de estilos e a ausência de CSS em linha. A validação formal dos ficheiros HTML e CSS está registada no ponto 5 deste relatório.

## Ponto 3 — Organização da folha CSS

A folha [`../css/style.css`](../css/style.css) foi organizada em 11 secções comentadas: cores, regras base, navegação, página inicial, secções e cartões, páginas interiores, rodapé, formulário, foco e acessibilidade visual, e adaptações para ecrãs estreitos. A folha contém mais de 15 regras CSS. A reorganização preserva as declarações e os valores de estilo existentes.

**Ponto 3 da E3: cumprido por inspeção do código.** A validação formal da sintaxe CSS fica para o ponto 5.

## Ponto 4 — Contraste da paleta

Em 25-10-2026, foram calculados os rácios dos pares de texto e fundo indicados na [guia de estilo](./guia-estilo.md), usando a fórmula de luminância relativa do WCAG. Os nove pares de texto registados apresentam rácio mínimo de 6,26:1; assim, todos ultrapassam 4,5:1 para texto normal e 3:1 para texto grande. O dourado usado no foco do rodapé sobre fundo castanho apresenta 5,99:1.

As cores laranja, dourado e linha foram identificadas na guia como cores decorativas/contorno, não como texto sobre fundos claros.

**Ponto 4 da E3: cumprido para os pares documentados na guia.**

## Ponto 5 — Validadores HTML e CSS

Validação realizada em 25-10-2026. Os cinco ficheiros HTML foram submetidos individualmente ao [Nu Html Checker](https://validator.w3.org/nu/). Todos terminaram sem erros nem avisos.

| Página | Resultado HTML | Captura |
|---|---|---|
| `index.html` | 0 erros, 0 avisos | [`w3c-E3-index.png`](./evidencias/w3c-E3-index.png) |
| `menu.html` | 0 erros, 0 avisos | [`w3c-E3-menu.png`](./evidencias/w3c-E3-menu.png) |
| `sobre.html` | 0 erros, 0 avisos | [`w3c-E3-sobre.png`](./evidencias/w3c-E3-sobre.png) |
| `contactos.html` | 0 erros, 0 avisos | [`w3c-E3-contactos.png`](./evidencias/w3c-E3-contactos.png) |
| `acessibilidade.html` | 0 erros, 0 avisos | [`w3c-E3-acessibilidade.png`](./evidencias/w3c-E3-acessibilidade.png) |

A folha [`../css/style.css`](../css/style.css) foi submetida ao [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/), com o perfil CSS Level 3 + SVG. O resultado foi **0 erros** e **3 avisos** informativos: o validador não verifica estaticamente variáveis CSS dinâmicas (linhas 157, 274 e 329). A captura do resultado está em [`w3c-E3-css.png`](./evidencias/w3c-E3-css.png).

**Ponto 5 da E3: cumprido — os validadores HTML e CSS reportaram 0 erros.**
