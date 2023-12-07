# HomePage Component

## Overview

O componente `HomePage` é uma página principal de um aplicativo de restaurante, apresentando uma lista de pratos disponíveis. Ele utiliza a biblioteca `styled-components` para estilização e `axios` para possíveis requisições HTTP.

## Estrutura

### Componentes Utilizados

- `Navbar`: Um componente que representa a barra de navegação.
- `Prato`: Um componente representando um prato individual na lista. Este componente ainda não está definido no código fornecido.

### Importações

- `styled` de `styled-components` para criar componentes estilizados.
- Imagens de pratos de diferentes diretórios.
- `useEffect` do React (não usado no exemplo fornecido).
- `axios` para possíveis requisições HTTP.

## JSX Structure

O JSX do componente `HomePage` é estruturado da seguinte forma:

- Um componente `Navbar`.
- Um container `ul` que lista três `Prato`, cada um passando uma imagem diferente como propriedade.

## Estilos CSS

### Container

Definido com um fundo escuro, estilo flex, e altura ajustada para ocupar a altura da viewport menos um valor fixo.

### Prato

Cada `Prato` é um item de lista com estilização própria:

- Fundo com uma imagem passada via props.
- Títulos e preços estilizados com cores específicas e espaçamento de letra.
- Um botão estilizado para mais informações.

---

## Exemplo de Uso

```jsx
import React from 'react';
import { HomePage } from './HomePage'; // Caminho de importação apropriado

function App() {
  return (
    <div className="App">
      <HomePage />
    </div>
  );
}

export default App;
```
