# Admin Marcafut

Bem-vindo à documentação do Admin Marcafut.

Nesta seção, você encontrará informações detalhadas sobre todas as configurações e funcionalidades disponíveis no Admin Marcafut.

---

## Repositório GitLab

Para acessar o código-fonte do Admin Marcafut, você pode visitar o repositório no GitLab:

[Repositório GitLab](https://gitlab.com/equipe-marcafut/marcafut-admin-react.git)

---

## Documentação do Template

O Admin Marcafut é baseado em um template para frontend. Abaixo, você encontrará links para a documentação e o demo do template:

- [Documentação do Template](https://www.creative-tim.com/learning-lab/react/overview/material-dashboard/)
- [Demo do Template](https://demos.creative-tim.com/material-dashboard-react/?&_ga=2.243368389.1789960355.1710330510-1339645420.1710330510#/dashboard)

Consulte a documentação do template para obter mais informações sobre sua estrutura e funcionalidades.

--- 
## Tecnologias Necessárias

Para rodar o projeto localmente, é necessário ter as seguintes tecnologias instaladas:

- [Node.js](https://nodejs.org/): versão 20.11.1 ou superior
- [npm (Node Package Manager)](https://www.npmjs.com/): versão 10.2.4 ou superior

Certifique-se de ter essas tecnologias instaladas em seu sistema antes de prosseguir.

---
# Estrutura do Projeto

O projeto é estruturado da seguinte forma:

- **src/assets**: Esta pasta contém temas, imagens e outros recursos que já fazem parte do template.

  > **Nota**: Conforme o desenvolvimento do projeto avança, vamos limpar esta pasta para deixá-la o mais enxuta possível.

- **src/components**: Aqui estão localizados os componentes que serão usados no projeto. Novos componentes serão criados nesta pasta.

- **src/components**: é responsável por gerenciar os estados globais dos componentes no projeto utilizando o contexto do React. Ele define um contexto principal chamado MaterialUIContext, que armazena e controla vários estados utilizados pelo projeto.

O contexto é utilizado para controlar configurações e funcionalidades globais do aplicativo, como a miniatura da barra lateral, a transparência da barra lateral e da barra de navegação, a cor da barra lateral, o layout, o modo escuro, entre outros.

O arquivo também exporta um provedor de contexto chamado MaterialUIControllerProvider, que envolve toda a aplicação e fornece o contexto MaterialUI para todos os componentes filhos. Além disso, ele exporta um hook personalizado chamado useMaterialUIController, que pode ser utilizado para acessar e modificar os estados globais em qualquer componente que esteja dentro do MaterialUIControllerProvider.

Os estados globais podem ser modificados utilizando as funções exportadas no arquivo, como setMiniSidenav, setTransparentSidenav, setSidenavColor, entre outras. Essas funções são usadas para despachar ações para o reducer definido no arquivo, que por sua vez atualiza o estado global com base na ação despachada.


- **src/examples**: Este diretório contém uma série de exemplos de componentes que podem ser utilizados no projeto. Cada subdiretório dentro de `examples` representa um tipo específico de componente ou conjunto de componentes, como Breadcrumbs, Cards, Charts, Configurator, Footer, Items, LayoutContainers, Lists, Navbars, Sidenav, Tables e Timeline.

  Dentro de cada subdiretório,  contêm a implementação desses componentes ou exemplos de uso. Por exemplo, dentro do diretório `Cards`, encontramos subdiretórios como `BlogCards`, `InfoCards`, `MasterCard`, `ProjectCards` e `StatisticsCards`, cada um contendo diferentes tipos de cartões de exemplo.

  Esses exemplos podem servir como referência para o desenvolvimento de novos componentes ou para entender como os componentes existentes são implementados.

- **src/layouts**: Este diretório contém diferentes layouts de páginas que podem ser usados no projeto. Cada subdiretório dentro de `layouts` representa um tipo específico de layout, como autenticação, faturamento, dashboard, notificações, perfil, rtl (para suporte a idiomas da direita para a esquerda) e tabelas.

  Dentro de cada subdiretório de layout, há arquivos que contêm a implementação dos componentes que compõem esse layout específico. Por exemplo, dentro do diretório `authentication`, encontramos componentes como `BasicLayout`, `CoverLayout`, `Footer`, `reset-password`, `sign-in` e `sign-up`, que são usados para definir o layout das páginas de autenticação do aplicativo.

  >**Nota**: Tem diretorios que não iremos usar, ou fazer modificações no decorrer do desevolvimento do sistema.

### **App.js**

O arquivo `App.js` é responsável por definir a estrutura principal da aplicação React, incluindo o layout, tema, configurações globais e navegação.

#### Funcionalidades Principais:

- **Inicialização**: Configura o estado global da aplicação e inicializações iniciais, como temas, direção (LTR ou RTL), layout e modo escuro.
- **Manipulação de Eventos**: Inclui funções para lidar com eventos, como onMouseEnter e onMouseLeave, que controlam a exibição da barra lateral em miniatura.
- **Configuração do Tema**: Define o tema da aplicação com base nas configurações de modo escuro e direção.
- **Renderização de Componentes**: Renderiza os componentes principais da aplicação, como a barra lateral, o configurador e as rotas usando o React Router.
- **Gestão de Estado**: Utiliza o contexto do React para gerenciar o estado global da aplicação e suas alterações ao longo do ciclo de vida.

Esse arquivo desempenha um papel fundamental na estrutura e funcionamento da aplicação React.

### **index.js**

O arquivo `index.js` é responsável por inicializar a aplicação React no navegador.
Funcionalidades Principais:

-   **Inicialização da Aplicação**: Utiliza o método createRoot do pacote react-dom/client para criar o ponto de entrada da aplicação no DOM.
-   **Configuração do Roteamento**: Utiliza o componente BrowserRouter do React Router para fornecer o roteamento da aplicação.
-   **Fornecimento do Contexto**: Utiliza o componente MaterialUIControllerProvider do contexto Material UI para fornecer o contexto global da aplicação.
-   **Renderização do Componente Principal**: Renderiza o componente principal App, que define a estrutura e o comportamento da aplicação.


### **routes.js**

O arquivo `routes.js` contém a definição de todas as rotas da aplicação Material Dashboard 2 React.

#### Funcionalidades Principais:

- **Definição de Rotas**: Todas as rotas da aplicação são adicionadas e configuradas neste arquivo. Cada rota é representada por um objeto no array `routes`.
- **Configuração de Layouts**: Cada rota especifica o layout correspondente que será renderizado quando a rota for acessada.
- **Configuração de Ícones**: Cada rota possui um ícone associado, que é exibido na barra lateral da aplicação.
- **Configuração de Componentes**: Cada rota especifica o componente correspondente que será renderizado quando a rota for acessada.
- **Roteamento**: As rotas são utilizadas pelo React Router para gerenciar a navegação da aplicação.
- **Tipos de Itens**: O arquivo define diferentes tipos de itens de rota, como colapsíveis, títulos e divisores, para organizar a estrutura da barra lateral da aplicação.



---



# Rodando o Projeto Local 

Scripts Disponíveis
No diretório do projeto, você pode executar:

```npm start```

Inicia o aplicativo no modo de desenvolvimento.
Abra http://localhost:3000 para visualizá-lo no seu navegador.
A página será recarregada quando você fizer alterações.
Você também pode ver quaisquer erros de lint no console.

`npm test`

Inicia o executor de testes no modo interativo de observação.
Consulte a seção sobre a execução de testes para mais informações.

`npm run build`

Compila o aplicativo para produção na pasta build.
Ele agrupa corretamente o React em modo de produção e otimiza a compilação para obter o melhor desempenho.
A compilação é minimizada e os nomes de arquivo incluem os hashes.
Seu aplicativo está pronto para ser implantado!
Consulte a seção sobre implantação para mais informações.

