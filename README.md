## Bikcraft

Este repositório é um site estático de loja/marketing da Bikcraft, uma marca que vende bicicletas elétricas personalizadas. Ele é estruturado em páginas de apresentação para home, bicicletas, seguros, contato, orçamento e termos, com um visual premium e forte identidade de produto.

### Stack
- Linguagens: HTML, CSS e JavaScript
- Framework / runtime: site estático puro; sem framework ou backend
- Bibliotecas notáveis: não há framework de aplicação; o comportamento principal vem de JavaScript customizado e de um plugin leve de animação (`js/plugins/simple-anime.js`)

## Como está organizado

```text
index.html              Página inicial com hero, bicicletas em destaque, benefícios, depoimentos e preços
bicicletas.html         Catálogo de bicicletas / página de listagem de produtos
bicicletas/             Páginas de detalhes dos modelos (magic, nimbus, nebula)
contato.html            Página de contato
orcamento.html          Página de orçamento / solicitação de cotação
seguros.html            Planos de seguros e preços
termos.html             Termos e condições
css/                    Estilos divididos por seção e camada utilitária
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
  plugins/              helper de animação
img/                    logos, fotos de bicicletas, ícones, parceiros e artes gráficas
favicon.svg             favicon da marca
```

**Como tudo se conecta:** O site é composto por páginas HTML independentes que compartilham um sistema de CSS comum e uma camada pequena de JavaScript. A página inicial reúne a apresentação e os produtos; as páginas de modelos ficam em `bicicletas/`; e o `js/script.js` adiciona interações como abrir/fechar FAQ e manter o estado de seleção de produto com base nos parâmetros da URL.

## Como executar

Como é um site estático, não há etapa de build nem instalação de dependências.

```bash
cd bikcraft
python3 -m http.server 8000
# depois abra http://localhost:8000
```

Você também pode abrir o arquivo `index.html` diretamente no navegador, mas um servidor local é a opção mais segura para caminhos de assets e comportamento do browser.

## Perguntas que você pode fazer

- “Quais arquivos CSS definem o tema visual e os tokens de design da marca?”
- “Como funciona a interação do FAQ em `js/script.js` junto com o HTML?”
- “As páginas de detalhes de bicicletas em `bicicletas/` foram pensadas como páginas estáticas individuais ou como algo que poderia ser gerado depois a partir de um CMS?”
