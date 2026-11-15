# Pastelaria Crumbly

## Elementos do grupo
- Fernando Augusto, nº 22410114
- José Leite, nº 22607530
- Gonçalo Ribeiro, nº 22206607


## Tema
Desenvolvimento de um sítio Web para uma pastelaria fictícia
portuguesa, dedicada à venda de pão fresco, bolos,
produtos de pastelaria e café.

## Público-alvo
Público em geral, incluindo famílias, estudantes e
trabalhadores que procuram produtos de padaria,
pastelaria e café.

## Objetivo do projeto
Criar um sítio Web acessível, responsivo e fácil de navegar,
que apresente os produtos e a identidade da Pastelaria Crumbly.

## Páginas iniciais da E1
- index.html — página inicial
- menu.html — produtos e preços
- sobre.html — apresentação da pastelaria

## Trabalho realizado por entrega

### E2 — Planeamento e formulários
- Foram acrescentadas as páginas `contactos.html` e `acessibilidade.html` e criada uma navegação comum nas cinco páginas.
- O formulário demonstrativo usa controlos HTML e validação nativa do navegador; não envia nem guarda dados.
- O planeamento e os testes estão descritos em [`docs/planeamento-E2.md`](docs/planeamento-E2.md) e [`docs/checklist-E2.md`](docs/checklist-E2.md).

### E3 — CSS base e validação
- As cinco páginas usam a folha de estilos externa `css/style.css`.
- Foram documentados a identidade visual e o contraste em [`docs/guia-estilo.md`](docs/guia-estilo.md) e os resultados de validação em [`docs/relatorio-validacao-E3.md`](docs/relatorio-validacao-E3.md).

### E4 — Modelo de caixa e layout
- O CSS usa regras de box model e layout responsivo, com estilos coerentes para tabelas e formulário.
- Foram acrescentados elementos HTML5, um artigo e documentação de teste de teclado em [`docs/checklist-E4.md`](docs/checklist-E4.md) e [`docs/artigo-E4/artigo.md`](docs/artigo-E4/artigo.md).

### E5 — Design responsivo
- O layout segue uma abordagem mobile-first, com três pontos de rutura, navegação flexível e grelha de conteúdos.
- Foram verificadas as cinco páginas a 360 px e 1280 px; as capturas estão em [`docs/responsivo/`](docs/responsivo/README.md).
- As imagens de conteúdo adaptam-se à largura do ecrã e os controlos principais têm áreas de toque com pelo menos 24 × 24 px.

### E6 — Bootstrap e auditoria inicial
- O Bootstrap CSS 5.3.9 é carregado por CDN; a paleta e os componentes são personalizados em `css/bootstrap-custom.css`, sem alterar os ficheiros do framework.
- A grelha Bootstrap está integrada nas páginas inicial e menu. Os componentes usados nesta etapa são cartões, botões, alerta, badge e tabelas.
- A primeira versão do artigo está em [`docs/artigo-E6/artigo-v1.md`](docs/artigo-E6/artigo-v1.md); o relatório em [`docs/relatorio-auditoria-E6.md`](docs/relatorio-auditoria-E6.md) regista os resultados Lighthouse e WAVE após as correções nas três páginas auditadas. As capturas Lighthouse são em modo Mobile e o WAVE reporta zero alertas.

## Tecnologias
- HTML5
- CSS
- Bootstrap CSS 5.3.9, carregado por CDN e personalizado em `css/bootstrap-custom.css`
- Git e GitHub

O projeto continua sem JavaScript próprio, bases de dados ou código de servidor. Nesta primeira etapa da E6, o Bootstrap é usado apenas como framework CSS.
