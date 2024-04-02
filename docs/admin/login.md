# Componente de Login Básico

O componente `Basic` é responsável por renderizar um formulário de login básico.

## Dependências

- react-router-dom: para a navegação do link.
- @mui/material: para os componentes de material UI.
- Material Dashboard 2 React: para alguns componentes específicos do Material Dashboard.

## Props

- `image` (string): A imagem de fundo a ser exibida na tela de login.

## Funcionalidades

- O componente inclui campos de entrada para nome de usuário e senha.
- Ele oferece a opção de lembrar as credenciais do usuário.
- Possui um botão de login para enviar as informações de login.
- Possui um componente para visualizar ou esconder a senha na hora da digitação.

---

- No login do administrador (`admin`), não haverá opção para criar senha ou recuperar senha. Essas funcionalidades podem ser adicionadas posteriormente, se necessário.

> **Nota** Dentro do diretório `authentication`, encontramos os seguintes subdiretórios e componentes:
>
> ### BasicLayout
>
> Este diretório contém o componente `index.jsx`, que representa o layout básico para a página de login.
>
> ### CoverLayout
>
> O diretório `CoverLayout` contém o componente `index.js`, que define o layout de capa para a página de login.
>
> ### Footer
>
> Este diretório inclui o componente `index.jsx`, responsável por exibir o rodapé na página de login.

### Testes

- Os testes para o componente de login básico estão localizados em `src/layouts/authentication/__tests__/Basic.tests.jsx`. Esses testes verificam se o formulário de login é renderizado corretamente com os campos de entrada, o switch de lembrar-me e o botão de login.
  
- O teste verifica se o formulário de login é renderizado corretamente com os campos de entrada, o switch de lembrar-me e o botão de login.
- Ele é executado usando Jest e @testing-library/react.
- Os elementos essenciais do formulário de login são verificados para garantir sua presença na tela.
- Outras funcionalidades interativas, como interações com o switch de lembrar-me, podem ser adicionadas e documentadas em testes adicionais.
