# Documentação Marcafut

Bem-vindo à documentação oficial do projeto Marcafut. Aqui, detalhamos meticulosamente todo o fluxo de trabalho, os testes realizados, os componentes utilizados e os endpoints para nossa API.

## Propósito

Nosso objetivo é fornecer uma visão abrangente de todas as etapas do desenvolvimento, garantindo uma compreensão clara de cada aspecto do projeto Marcafut. Desde o planejamento até a implantação, você encontrará informações detalhadas para facilitar o desenvolvimento, manutenção e integração de nossos produtos.

## Repositório GitLab

Todo o código-fonte do projeto Marcafut está hospedado em nossos repositórios no GitLab. Cada um de nossos produtos possui seu próprio repositório dedicado, permitindo uma gestão eficiente do versionamento e colaboração entre equipes.

## Tecnologias Utilizadas

Nossa stack tecnológica é diversificada e adaptada às necessidades específicas de cada componente do projeto. Entre as tecnologias utilizadas, destacam-se o React para o desenvolvimento dos produtos Web e Java para a API, entre outras ferramentas e bibliotecas que contribuem para a robustez e eficiência do projeto.

## Produtos

### Web

- **Admin**: O Admin é responsável por todas as configurações do sistema, incluindo o cadastro de novos centros esportivos, configurações de agenda, logs e muito mais.
  
- **CE Web (Central do Esportista)**: A CE Web é uma plataforma onde os proprietários de centros esportivos podem gerenciar seus estabelecimentos. Eles podem marcar horários, gerenciar os fluxos, criar aulas, ver os indicadores financeiros e muito mais.
  
- **Jogador Web**: A versão Web para jogadores permite que os usuários visualizem os centros esportivos, realizem agendamentos e executem outras funções (ainda em desenvolvimento).

### Mobile

- **App CE**: O App CE oferece as mesmas funcionalidades da CE Web, com notificações nativas no celular, proporcionando uma experiência ainda mais fluida e conveniente.

- **App Jogador**: O App Jogador é uma versão mais completa da versão Web para jogadores. Os jogadores podem realizar o cadastro, acessar a localização da arena, acessar as redes sociais da arena, realizar agendamentos e receber notificações nativas, proporcionando uma experiência completa e integrada.

Com esta documentação, esperamos oferecer uma visão completa e acessível do projeto Marcafut, proporcionando uma base sólida para desenvolvedores e equipes envolvidas em seu desenvolvimento e manutenção.


## Testes

Nossa abordagem de testes para o projeto Marcafut é abrangente e inclui tanto testes unitários quanto testes de interface do usuário (UI). Utilizamos duas ferramentas principais para nossos testes: Jest e Cypress.

### Jest

O Jest é uma estrutura de teste de JavaScript desenvolvida pelo Facebook. Ele é amplamente utilizado para testes unitários em aplicativos React, e é uma escolha popular devido à sua simplicidade e poderosas funcionalidades de assertivas.

#### O que o Jest faz:

- Testes unitários: Jest é ideal para escrever e executar testes unitários em componentes individuais, funções e lógica de negócios.
- Mocking: Jest fornece uma ampla gama de recursos para simular o comportamento de módulos, permitindo testes isolados e independentes.
- Cobertura de código: Jest possui suporte integrado para medir a cobertura de código, ajudando a garantir que todas as partes do código estejam sendo testadas adequadamente.

### Cypress

O Cypress é uma ferramenta de teste de ponta a ponta (end-to-end) desenvolvida para testar aplicativos da web modernos. Ele oferece uma experiência de desenvolvimento de testes fácil de usar e poderosa, permitindo testes interativos e automatizados em ambientes reais de aplicativos da web.

#### O que o Cypress faz:

- Testes de interface do usuário (UI): Cypress é projetado especificamente para testar a interface do usuário de aplicativos da web, permitindo interações com elementos da página e validação visual.
- Testes de ponta a ponta: Cypress permite simular fluxos de usuário completos, desde ações de navegação até a entrada de dados em formulários e verificações de resultados.
- Facilidade de uso: Cypress oferece uma API intuitiva e uma interface de usuário amigável para escrever, depurar e executar testes de forma eficiente.

Combinando Jest para testes unitários e Cypress para testes de interface do usuário, garantimos uma cobertura abrangente de nossos produtos, ajudando a garantir a qualidade e a confiabilidade do projeto Marcafut.

## Executando Testes

O Jest é a ferramenta padrão para execução de testes em projetos JavaScript/Node.js. Ele automaticamente busca por arquivos de teste com os sufixos `.test.js`, `.spec.js`, ou que estão dentro de pastas com o nome `__tests__` e os executa quando o comando `npm test` é acionado.

Para executar os testes do projeto, basta abrir um terminal na raiz do projeto e digitar o seguinte comando:

    npm test


Isso fará com que o Jest procure por todos os arquivos de teste no projeto e execute-os, fornecendo feedback sobre o sucesso ou falha dos testes.

>Certifique-se de que todas as dependências necessárias estejam instaladas e que os arquivos de teste estejam corretamente organizados de acordo com as convenções do Jest para garantir que os testes sejam executados com sucesso.
