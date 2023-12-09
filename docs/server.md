# Documentação do Servidor Flask com SQLAlchemy

Esta documentação detalha a implementação de um servidor Flask que utiliza SQLAlchemy para interação com um banco de dados MySQL. O servidor oferece APIs para gerenciar usuários, produtos, restaurantes e pesquisas de produtos e restaurantes.

## Configuração Inicial

- **Flask**: Framework utilizado para criar o servidor web.
- **SQLAlchemy**: ORM (Object-Relational Mapping) utilizado para interagir com o banco de dados MySQL.
- **Flask_CORS**: Utilizado para habilitar o Cross-Origin Resource Sharing (CORS).
- **mysql.connector**: Conector para MySQL.
- **JSON**: Formato de dados para as respostas da API.

## Modelos de Dados

- **usuarios**: Representa usuários, com campos para ID, nome, função, login e senha.
- **produtos**: Representa produtos, com campos para ID, nome, ID do restaurante, preço, descrição e imagem.
- **restaurantes**: Representa restaurantes, com campos para ID, nome, distância e logo.
- **pesquisas_produto** e **pesquisas_restaurante**: Representam pesquisas realizadas por produtos e restaurantes, respectivamente.

## Endpoints da API

1. **Usuários**:
   - `GET /usuarios`: Retorna todos os usuários.
   - `GET /usuario/<id_usuario>`: Retorna um usuário específico pelo ID.
   - `POST /usuarios`: Cria um novo usuário.
   - `PUT /usuario/<id_usuario>`: Atualiza um usuário existente.
   - `DELETE /usuario/<id_usuario>`: Deleta um usuário.

2. **Produtos**:
   - `GET /produtos`: Retorna todos os produtos.
   - `GET /produto/<id_produto>`: Retorna um produto específico pelo ID.
   - `POST /produtos`: Cria um novo produto.
   - `PUT /produto/<id_produto>`: Atualiza um produto existente.
   - `DELETE /produto/<id_produto>`: Deleta um produto.

3. **Restaurantes**:
   - `GET /restaurantes`: Retorna todos os restaurantes.
   - `GET /restaurante/<id_restaurante>`: Retorna um restaurante específico pelo ID.
   - `POST /restaurantes`: Cria um novo restaurante.
   - `PUT /restaurante/<id_restaurante>`: Atualiza um restaurante existente.
   - `DELETE /restaurante/<id_restaurante>`: Deleta um restaurante.

4. **Pesquisas**:
   - `GET /pesquisas_produto`: Retorna todas as pesquisas de produtos.
   - `GET /pesquisa_produto/<id_pesquisa_produto>`: Retorna uma pesquisa de produto específica.
   - `POST /pesquisas_produto`: Cria uma nova pesquisa de produto.
   - `PUT /pesquisa_produto/<id_pesquisa_produto>`: Atualiza uma pesquisa de produto.
   - `DELETE /pesquisa_produto/<id_pesquisa_produto>`: Deleta uma pesquisa de produto.
   - `GET /pesquisas_restaurante`: Retorna todas as pesquisas de restaurantes.
   - `GET /pesquisa_restaurante/<id_pesquisa_restaurante>`: Retorna uma pesquisa de restaurante específica.
   - `POST /pesquisas_restaurante`: Cria uma nova pesquisa de restaurante.
   - `PUT /pesquisa_restaurante/<id_pesquisa_restaurante>`: Atualiza uma pesquisa de restaurante.
   - `DELETE /pesquisa_restaurante/<id_pesquisa_restaurante>`: Deleta uma pesquisa de restaurante.

5. **Pesquisa Avançada**:
   - `GET /pesquisar_restaurantes/<nome_restaurante>`: Pesquisa restaurantes pelo nome.
   - `GET /pesquisar_prato/<nome_produto>`: Pesquisa produtos pelo nome.
   - `GET /filtrar_maior_distancia`: Lista restaurantes por ordem decrescente de distância.
   - `GET /filtrar_menor_distancia`: Lista restaurantes por ordem crescente de distância.
   - `GET /filtrar_menor_preco`: Lista produtos por ordem crescente de preço.
   - `GET /filtrar_maior_preco`: Lista produtos por ordem decrescente de preço.

## Erro Handling

- `@app.errorhandler(404)`: Um manipulador de erros personalizado para a rota 404 (página não encontrada).

## Execução do Servidor

- `app.run()`: Inicia o servidor Flask.

## Uso

O servidor pode ser utilizado para criar um sistema

 de gestão de restaurantes e produtos, onde usuários podem realizar pesquisas e gerenciar informações relevantes. Ele oferece uma API RESTful para a interação com um banco de dados de restaurantes e produtos.