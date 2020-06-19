---
layout: page
title: Quero contribuir com este blog
permalink: /contribuir/
---

## Formas de contribuir

- Você pode contriuir com pull-requests
  - Realizando uma correção no site
  - Resolvendo uma issue
  - Criando um post
  - Criando uma apresentação de slides
  - Adicionando alguma nova funcionalidade
- Encontrando problemas e erros (erros de digitação, página com problema, informação incorreta)
  - Abrir uma issue no repositório: [ProfPetroski/workshop_git Issues](https://github.com/ProfPetroski/workshop_git/issues)
  - Comentários e contribuições nas discussões já existentes

### Abrir pull-requests

- Realizar o fork deste repositório: [ProfPetroski/workshop_git](https://github.com/ProfPetroski/workshop_git)
- Fazer o download do seu repositorio
- Realizar as alterações desejadas no seu repositoório
- Fazer o pull request das suas alterações no repositório [ProfPetroski/workshop_git](https://github.com/ProfPetroski/workshop_git)

## Estrutura do blog
- O blog foi desenvolvido com [Jekyll ](https://jekyllrb.com/docs/)
- As [Apresentações de slides](/listaapresentacoes) foram desenvolvidas com [remarkjs](https://github.com/gnab/remark)
- O tema utilizado é [chrisrhymes/bulma-clean-theme](https://github.com/chrisrhymes/bulma-clean-theme)

### Estrutura de diretórios
```bash
/docs
├── _config.yml
├── _data
│   └── navigation.yml
├── _includes
│   ├── latest-posts.html
│   └── post-card.html
├── _layouts
│   ├── slides.html
├── _posts
│   └── 2020-06-18-bem-vindo.md 
├── _slides
│   └── workshop_git.html
├── assets
│   ├── css
│   ├── img
│   └── js
├── 404.html
├── about.md
└── index.md 
```

| Arquivo/Diretorio | Descrição                                                                                                                                                                                                                                                                                                                                                                        |
|-------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| docs              | Este é o diretório para armazenar o blog estático. As configurações do GitHub Pages foram adicionadas para utilizar o diretório /docs da branch master para servir o site. As páginas podem ser criadas neste diretório, como por exemplo a página inicial (index.md) e o Sobre (about.md)                                                                                       |
| _config.yml       | Armazena as configurações do site.                                                                                                                                                                                                                                                                                                                                               |
| _data             | Armazena lista de informações gerais do site. Neste site está armazenado o menu superior. Pode armazenar qualquer agregado de informações com a extensão yml, yaml, csv tsv ou json. O conteúdo pode ser acessado através da variável site.data.<nome_do_arquivo>                                                                                                                |
| _includes         | Diretório utilizado para criar partes da página que deverá ser composta nos layouts. Por exemplo: Menu, lista de posts, etc. Quando se utiliza um tema (theme), este já possui os includes, porém pode ser sobrescrito os arquivos do tema neste diretório.                                                                                                                      |
| _layouts          | Definição dos templates de páginas. No caso de utilização de um tema (theme) ele já possui os layouts pré-definidos. Porém neste diretório podem ser estendidos novos layouts, assim como sobrescrever os layouts já existentes do tema                                                                                                                                          |
| _posts            | Neste diretório são armazenados os conteúdos dinâmicos do blog (posts). Os arquivos deste diretório devem seguir o seguinte padrão de nomenclatura: ANO-MÊS-DIA-titulo.md                                                                                                                                                                                                        |
| _slides           | Neste diretório podem ser criadas apresentações de slides. Estas apresentações serão listadas no menu Páginas > Apresentações. Para criar as apresentações devem ser aplicado o layout slides:  <br><code> ---<br> layout: slides<br> title: Workshop Introdução ao GIT<br>---<br> </code> O conteúdo dos slides deve serguir a documentação do [remark Wiki](https://github.com/gnab/remark/wiki) |
| assets            | Utilizado para armazenar o conteúdo estático de css, imagens e javascript                                                                                                                                                                                                                                                                                                        |

