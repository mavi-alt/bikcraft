# Bikcraft

Site estático de marketing e vendas da Bikcraft, uma marca que comercializa bicicletas elétricas personalizadas. O projeto foi estruturado como uma landing page e um conjunto de páginas institucionais, com foco em apresentação visual, conversão e navegação simples.

## Sobre o projeto

Este repositório reúne o front-end estático da Bikcraft, com páginas para:
- home
- catálogo de bicicletas
- páginas de detalhes dos modelos
- orçamento
- contato
- seguros
- termos e condições

A estrutura foi organizada para facilitar manutenção com CSS modularizado e um script leve para interações do cliente.

## Stack

- HTML5
- CSS3
- JavaScript
- Animações leves com plugin customizado em `js/plugins/simple-anime.js`

## Funcionalidades

- Layout responsivo para desktop, tablet e mobile
- Página inicial com destaque de produtos e benefícios
- Catálogo de bicicletas com páginas detalhadas
- Seção de seguros com planos e FAQ
- Formulário de orçamento
- Navegação clara entre páginas
- Interações simples com JavaScript, como:
  - FAQ
  - seleção de produto
  - galeria de bicicletas
  - navegação ativa no menu

## Estrutura do projeto

```text
index.html              Página inicial com hero, bicicletas em destaque, benefícios, depoimentos e preços
bicicletas.html         Catálogo de bicicletas / página de listagem
bicicletas/             Páginas de detalhes dos modelos (magic, nimbus, nebula)
contato.html            Página de contato
orcamento.html          Página de orçamento / solicitação de cotação
seguros.html            Planos de seguros e preços
termos.html             Termos e condições
css/                    Estilos organizados por seção e utilitários
  global/               layout base, cabeçalho, rodapé
  home/                 estilos da página inicial
  bicicletas/           estilos do catálogo
  bicicleta/            estilos dos detalhes dos produtos
  seguros/              estilos de seguros e FAQ
  contato/              estilos da página de contato
  orcamento/            estilos do formulário de orçamento
  termos/               estilos dos termos
  utilidades/           tipografia, cores, botões, formulários compartilhados
js/                     interações do lado do cliente
  script.js             FAQ, menu ativo, seleção de produto e galeria de bicicletas
  plugins/              helpers de animação
img/                    logos, fotos de bicicletas, ícones, parceiros e artes gráficas
favicon.svg             favicon da marca
```
## Créditos

- Curso: Origamid — [HTML e CSS para Iniciantes](https://www.origamid.com/curso/html-e-css-para-iniciantes/)
