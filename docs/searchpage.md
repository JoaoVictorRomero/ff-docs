# Documentação da Página de Busca

Esta documentação fornece um guia detalhado sobre a funcionalidade e o código da `SearchPage`, uma página de busca de produtos implementada em React.

## Componentes Utilizados

- `React` (useState, useEffect): para gerenciar o estado e o ciclo de vida do componente.
- `axios`: para fazer requisições HTTP.
- Componentes customizados:
  - `Navbar`: um componente para a barra de navegação.
- Arquivos de estilo: `search.css` para estilização.

## Funcionalidade

A `SearchPage` permite aos usuários buscar produtos por nome e filtrar os resultados por categoria.

### Estados

- `value`: Mantém o estado da categoria selecionada (`'all'` por padrão).
- `dados`: Armazena os dados dos produtos recebidos do servidor.
- `searchText`: Armazena o texto atual da busca.

### Requisição de Dados

- A página faz uma requisição para um servidor local (`http://127.0.0.1:5000/produtos`) para obter dados dos produtos.
- Esta requisição é realizada no carregamento da página (`useEffect` com um array de dependências vazio).

### Interface do Usuário

- **Barra de Busca**: Permite que os usuários digitem um texto para buscar produtos.
- **Filtro de Categoria**: Permite que os usuários filtrem os produtos por categorias específicas como 'Entrada', 'Sobremesa', 'Prato Principal', ou 'Tudo'.
- **Exibição de Produtos**: Os produtos são listados em cartões, incluindo imagem, preço, nome, restaurante e descrição. Um filtro de texto e categoria é aplicado aos dados.

### Filtragem de Produtos

- A filtragem é feita em duas etapas:
  1. **Filtro de Texto**: Compara o texto da busca com o nome do produto.
  2. **Filtro de Categoria**: Compara a categoria selecionada com a descrição do produto.

## Estrutura do Código

O código está estruturado em uma função `SearchPage`, que retorna JSX. O JSX inclui a barra de navegação (`Navbar`), a seção de busca, e a seção de exibição de produtos. Dentro da seção de produtos, há uma lógica condicional para exibir os produtos filtrados ou uma mensagem de carregamento.

## Exemplo de Uso

```jsx
import React from 'react';
import { SearchPage } from './SearchPage';

function App() {
  return (
    <div className="App">
      <SearchPage />
    </div>
  );
}

export default App;
```
