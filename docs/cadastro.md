# Documentação das Páginas de Cadastro e Login

Esta documentação abrange duas páginas do projeto React: `SingUpPage` (Cadastro) e `SingInPage` (Login), explicando suas funcionalidades, estruturas e componentes.

## SingUpPage (Página de Cadastro)

### Componentes e Bibliotecas Utilizadas

- `React` (useState): para gerenciar o estado.
- `Navbar`: componente para a barra de navegação.
- `Link` de `react-router-dom`: para navegação.

### Funcionalidade

A página de cadastro permite que usuários se registrem como pessoa física ou restaurante. Se o usuário selecionar "Restaurante", campos adicionais para detalhes do restaurante são exibidos.

### Estados

- `showRestaurantFields`: Controla a exibição dos campos específicos para cadastro de restaurante.

### Lógica da Interface

- A página exibe um formulário com campos para nome, email e senha.
- Se `showRestaurantFields` for verdadeiro, campos adicionais para URL da imagem, latitude e longitude são exibidos.
- Um menu suspenso permite que o usuário escolha entre se registrar como "Pessoa Fisica" ou "Restaurante".
- O formulário é enviado para um servidor local (`http://127.0.0.1:5000/cadastro`).

## SingInPage (Página de Login)

### Componentes e Bibliotecas Utilizadas

- `React` (useState, useEffect): para gerenciar estados e o ciclo de vida do componente.
- `axios`: para fazer requisições HTTP.
- `useNavigate` de `react-router-dom`: para navegação programática.
- `Navbar`: componente para a barra de navegação.

### Funcionalidade

A página de login permite que usuários entrem no sistema usando seu email e senha.

### Estados

- `login` e `senha`: Armazenam os dados de entrada do usuário.
- `users`: Armazena os dados dos usuários obtidos do servidor.

### Lógica da Interface

- A página exibe um formulário para login com campos para email e senha.
- Os dados dos usuários são carregados do servidor na montagem do componente.
- O botão "Logar" envia o formulário e verifica as credenciais do usuário.
- Se as credenciais forem válidas, o usuário é redirecionado para a página inicial e suas informações são armazenadas no `localStorage`.

## Estilos

Ambas as páginas utilizam o arquivo de estilo `signIn-up.css` para a estilização dos formulários e conteúdo.

## Exemplo de Uso

Para incorporar essas páginas em um aplicativo React, importe e use-as dentro de um componente de roteamento:

```jsx
import React from 'react';
import { BrowserRouter as Router, Route, Routes } from 'react-router-dom';
import { SingUpPage, SingInPage } from './pages';

function App() {
  return (
    <Router>
      <Routes>
        <Route path="/SingUp" element={<SingUpPage />} />
        <Route path="/SingIn" element={<SingInPage />} />
      </Routes>
    </Router>
  );
}

export default App;
```

