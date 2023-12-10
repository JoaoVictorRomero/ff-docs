## Integrantes do Grupo:
- Enzo Matschinski Kummer - 222005377 - Product Owner
- Vinícius Gonçalves Duarte - 222026869 - Scrum Master 
- Marcelo Vitor Meira de Lucena - 221030034
- Gabriel Ribeiro da Silva - 222005401
- Weldo Gonçalves da Silva Junior - 222014133
- Rodrigo reis dos santos - 222026546 -
- Yuri Santana Lopes - 222009750
- João Victor das Neves Romero - 221028546
- Alan Henrique -190101270




## Historietas

- O usuário chegou no totem presente na Praça de Alimentação do shopping, onde se
  deparou com uma tela inicial que mostrava uma aba de pesquisa, um mapa, e logo
  abaixo, um pequeno “feed” com os principais pratos e promoções do dia;
- O usuário escolheu pesquisar, e então lhe foi aberta uma aba de pesquisa, onde ele
  filtrou o resultado por pratos ou restaurantes, distância e preço;
- O usuário pesquisou pelo nome do prato que deseja comer, e o totem lhe mostrou
  todas as opções de diferentes restaurantes que compreendem seu desejo,
  ordenados por distância geográfica. Ou, o usuário escreveu o restaurante que
  deseja pesquisar, e abriu uma aba do perfil do restaurante, com cardápio, distância
  do totem, etc.;
- O usuário selecionou o prato que deseja consumir e recebeu todas as informações
  necessárias para chegar até o restaurante, preço, estimativa de tempo de preparo,
  etc.;
- Após receber todas essas informações, é perguntado ao usuário se o mesmo deseja
  fazer login para salvar seus interesses e desejos. Caso o cliente deseje fazer login, o
  totem (aplicativo) exibe uma nova página, onde o usuário preenche seus dados
  (caso já tenha se cadastrado no sistema) ou escolhe criar um novo cadastro. Caso o
  usuário deseje criar, ele é direcionado para a tela de criação de cadastro, onde ele
  preenche com seu login e senha de preferência. Essas informações são então
  criptografadas e cadastradas no banco de dados;
- Após o processo de login (ou de dispensar esse processo), é perguntado ao usuário
  se ele é PcD (Pessoa com Deficiência) e precisa de ajuda para chegar até o
  restaurante. Caso o usuário selecione que sim, a equipe do shopping será alertada
  para que envie alguém;
- O staff do shopping possui um simples programa que os alerta quando alguma PcD
  necessita de ajuda, informando a localização do totem onde essa pessoa está.

- O administrador conferiu se todos os produtos listados estão corretos. Quando um
  restaurante foi à falência, o administrador removeu o restaurante da lista de
  restaurantes, assim como todos os seus dados do banco de dados.
- O administrador faz o cadastro de novos “totens” no sistema, informando sua
  localização geográfica. Ele também remove um totem do sistema, caso o mesmo
  seja retirado.

- O vendedor acessa a plataforma destinada aos vendedores para ali cadastrar seu
  restaurante com a localização geográfica
- Depois, o vendedor pode criar os pratos de seu restaurante, com preço, foto e tempo
  de preparo médio.
- O administrador aprova ou reprova a criação de perfil de um restaurante, assim
  como a página dos seus pratos.


## Ferramentas

### Linguagem:

Para o desenvolvimento do site, usaremos javascript, css e react.

- Usaremos o padrão do Google de codificação por javascript ([Guia de Estilo Google](https://google.github.io/styleguide/jsguide.html))
- Será usado ESLint como programa que irá verificar o padrão de codificação. ([ESLint](https://eslint.org))

### Framework de Teste:

- Como framework de teste, usaremos o JTest, que permite o teste de javascript e funciona bem com react.

### Bibliotecas e Frameworks Utilizadas:

- Bibliotecas e frameworks para o backend:
  - Flask
  - Flask_SQLAlchemy
  - MySQL-connector-python
  - MySQLclient
  - Flask-CORS
  - Pytest

### Verificador de Código:

- ESLint (verificador estático de Javascript e React)

### Sites Utilizados:

- GitHub (controle de versões)
- Trello (SCRUM/Kanban)

### Verificador de Cobertura:

- Plugin Cypress ([Cypress](https://www.cypress.io))

### Gerador de Documentação:
- Mkdocs




## Divisão das Ações por Historietas:

1° Sprint: 

- História: 01

2° Sprint (Mudança de Sistema): 

- Histórias: 01, 02, 03

3° Sprint (Integração): 

- Histórias: 04, 08, 11

4° Sprint: 

- Histórias: 05, 10, 12


!!! warning "EU01: Front-end"
    O usuário chegou no totem presente na Praça de Alimentação do shopping, onde se deparou com uma tela inicial que mostrava uma aba de pesquisa, um mapa, e logo abaixo, um pequeno “feed” com os principais pratos e promoções do dia.

!!! warning "EU02: Front-end"
    O usuário escolheu pesquisar, e então lhe foi aberta uma aba de pesquisa, onde ele filtrou o resultado por pratos ou restaurantes, distância e preço.

!!! warning "EU03: Front-end"
    O usuário pesquisou pelo nome do prato que deseja comer, e o totem lhe mostrou todas as opções de diferentes restaurantes que compreendem seu desejo, ordenados por distância geográfica. Ou, o usuário escreveu o restaurante que deseja pesquisar, e abriu uma aba do perfil do restaurante, com cardápio, distância do totem, etc.;

!!! warning "EU04: Front-end"
    O usuário selecionou o prato que deseja consumir e recebeu todas as informações necessárias para chegar até o restaurante, preço, estimativa de tempo de preparo, etc.


!!! tip "EU05: Sistema a ser implementado"
    Após receber todas essas informações, o usuário decide se quer fazer login para salvar preferências. Se optar pelo login, pode inserir dados já cadastrados ou criar um novo cadastro, onde as informações são criptografadas e armazenadas.

!!! danger "EU06: Removido do projeto"
    Questiona-se o usuário se ele é uma Pessoa com Deficiência (PcD) e requer assistência para navegar até o restaurante. Se afirmativo, a equipe do shopping é notificada para prestar auxílio.

!!! danger "EU07: Removido do projeto"
    O sistema de gestão do shopping recebe alertas quando usuários PcD necessitam de ajuda, mostrando a localização do totem utilizado.

!!! note "EU08: Back-end"
    O administrador verifica a correção dos produtos listados. Em caso de fechamento de um restaurante, ele o remove da listagem e do banco de dados.

!!! danger "EU09: Removido do projeto"
    O administrador cadastra novos totens no sistema e remove os que não estão mais em uso.

!!! note "EU01: Back-end"
    Vendedores acessam uma plataforma específica para cadastrar seus restaurantes, incluindo a localização geográfica.

!!! note "EU11: Back-end"
    Vendedores podem cadastrar pratos dos seus restaurantes, definindo preço, foto e tempo médio de preparo.

!!! tip "EU12: Sistema a ser implementado"
    O administrador tem a função de aprovar ou reprovar a criação de perfis de restaurantes e seus pratos.



## Backlog de Desenvolvimento

### Sprint 1

- **Desenvolvimento Front-end**: Implementação da tela inicial "Food Finder" com barra de navegação e abas para Buscar, Pratos do Dia e Mapa.

- **Desenvolvimento Back-end**: Criação do banco de dados com funcionalidades CRUD para usuários e restaurantes.

### Sprint 2

- **Transição para Web**: Mudança do sistema de Python para uma aplicação web usando JavaScript, CSS e React.

- **Reconstrução e Adições no Front-end**:
  - Reestruturação do front-end para ambiente web.
  - Adição de filtros de pesquisa por tipo de prato.
  - Inclusão de exemplos de produtos.
  - Desenvolvimento da função de mapa e da página "Pratos do Dia".

- **Funcionalidades CRUD para Pratos no Back-end**.

- **Observações**: Decisão de não incluir páginas individuais de restaurantes devido à complexidade e redundância com a funcionalidade de busca.

### Sprint 3

- **Página de Administrador e Dono de Restaurante**: Implementação de funcionalidades para adicionar, remover e editar pratos e restaurantes.

- **Melhorias na Interface**:
  - Adição de imagens aos pratos listados.
  - Implementação de um submenu para navegação entre páginas de Admin e Dono de Restaurante.

- **Mapa Interativo**: Desenvolvimento de um mapa interativo na página de mapas.

- **Atualização do Banco de Dados**: Inclusão de pratos por restaurante e links para imagens dos produtos.

### Sprint 4

- **Integração e Documentação**: Verificação da integração entre as funções da página de Admin e a listagem de restaurantes.

- **Funcionalidades de Filtragem**: Implementação da filtragem de restaurantes por distância.
