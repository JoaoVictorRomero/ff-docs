# Documentação da Página de Administração

Esta documentação descreve a `AdminPage`, uma página de administração desenvolvida em React, que fornece interfaces para adicionar e excluir restaurantes e pratos.

## Componentes Utilizados

- `React` (useState): Utilizado para gerenciar os estados da página.
- `styled-components`: Para estilizar os componentes.
- Componentes customizados:
  - `Navbar`: Componente para a barra de navegação.
  - `RestaurantMenu` e `RestaurantDishMenu`: Componentes para os menus de adição e exclusão de restaurantes e pratos.

## Funcionalidade

A `AdminPage` permite aos administradores adicionar ou excluir restaurantes e pratos através de menus modais.

### Estados

- `isAddMenuVisible` e `isDeleteMenuVisible`: Controlam a visibilidade dos menus de adicionar e excluir.

### Ações de Interface

- `toggleAddMenu` e `toggleDeleteMenu`: Funções para alternar a visibilidade dos menus de adicionar e excluir.
- `closeAddMenu` e `closeDeleteMenu`: Funções para fechar os menus de adicionar e excluir.

### Interface do Usuário

- A página exibe dois botões principais: um para adicionar e outro para excluir restaurantes.
- Ao clicar em cada botão, um menu modal correspondente é exibido.
- O menu de adição permite inserir o nome, URL da imagem e código de confirmação do restaurante.
- O menu de exclusão permite inserir o nome do restaurante para exclusão, código de confirmação e motivo.
- Um terceiro botão permite excluir um prato específico de um restaurante, exigindo o nome do restaurante, nome do prato, código de confirmação e motivo.

## Estrutura do Código

O código é organizado em uma função `AdminPage`, que retorna JSX contendo a barra de navegação (`Navbar`) e um container principal (`Containerdiv`). Dentro deste container, são exibidos os botões para adicionar e excluir, assim como os menus modais condicionais.

## Estilos

- Os estilos são definidos usando `styled-components`, permitindo uma fácil manutenção e legibilidade do código.
- `Containerdiv`, `H1`, `H2`, `Button`, `MenuContainer`, `InputBox`, `CloseButton` e `RestMenu` são estilizados de forma a criar uma interface visualmente agradável e funcional.

## Exemplo de Uso

```jsx
import React from 'react';
import { AdminPage } from './AdminPage';

function App() {
  return (
    <div className="App">
      <AdminPage />
    </div>
  );
}

export default App;
```

