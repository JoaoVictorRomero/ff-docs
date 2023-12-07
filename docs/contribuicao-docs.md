# Guia de Contribuição para a Documentação

## Estrutura de Arquivos

A organização do repositório é a seguinte:

```
.
├── docs
│   ├── (DIRETÓRIO DE IMAGENS)
│   ├── contribuicao-docs.md
│   ├── homepage.md
│   ├── index.md
│   └── (demais arquivos...)
└── mkdocs.yml
```

A pasta `docs` contém todos os documentos de texto e o arquivo `mkdocs.yml` define as configurações do site.

## Configurando o Ambiente

É utilizado o framework [Mkdocs](https://squidfunk.github.io/mkdocs-material/reference/) para gerar o site da documentação. É aconselhável ler a documentação oficial para entender todas as funcionalidades disponíveis. Além disso, é essencial conhecer a sintaxe do [Markdown](https://www.markdownguide.org/cheat-sheet/) para editar os arquivos `.md`.

Para começar, clone o [Repositório](https://github.com/JoaoVictorRomero/ff-docs):

```
git clone git@github.com:JoaoVictorRomero/ff-docs.git
```

Instale o Mkdocs Material com o comando:

```
pip install mkdocs-material
```

Para visualizar o site localmente, execute:

```
mkdocs serve
```

Agora, você pode acessar o site pelo link: [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## Editando a Documentação

### Adicionando Seções à Barra Lateral

O arquivo `mkdocs.yml` contém a estrutura de navegação sob a chave `nav`. Por exemplo:

```yaml
nav:
  - Sobre: "index.md"
  - Frontend:
    - HomePage: 'homepage.md'
  - Backend:
    - SLA: 'a.md'
  - Outros:
    - Contribuição para Docs: 'contribuicao-docs.md'
```

As seções de primeiro nível (ex. Sobre, Frontend) representam os títulos na barra lateral esquerda, enquanto as seções aninhadas representam as páginas de conteúdo dentro da pasta `docs`. Para adicionar uma nova página, insira o nome do arquivo correspondente no `mkdocs.yml`.

### Edição Direta

Para editar rapidamente, clique no ícone :material-file-edit: localizado no topo da página. Você será redirecionado para o arquivo da página no GitHub, onde poderá fazer alterações diretamente.

!!! note "Observação"
    Qualquer alteração feita na `main branch` será automaticamente publicada no site.
