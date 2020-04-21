## Lofi App
Plataforma com o principal objetivo de conectar jogadores de xadrez

### Requisitos Funcionais
- Playlists:
  - Poder criar uma nova playlist
  - Poder deletar uma playlist existente
  - Poder adicionar músicas à playlist existente
  - Poder ouvir playlists
  
- Músicas
  - Poder salvar uma música em uma das playlists
  - Poder remover uma música de uma playlist
  - Todas as músicas devem ser no estilo Lo-Fi
  
- Download de músicas
  - Poder fazer o download de uma música
  - Poder fazer download de uma playlist
  - Poder fazer download de um arquivo CSV com os dados de uma playlists e suas músicas
  
- Página de configurações
  - Possibilidade de trocar temas
  - Deve ter a opção de alternar temas além do light e dark
  - Possibilidade de alterar a tipografia (fonte)

- Páginas:
  - Página para configuração
  - Página para listar as playlists
  - Página para listar as músicas de uma playlist
  - Página para mostrar músicas aleatórias
  - Página para mostrar músicas de uma certeza subcategoria
  
  
### Requisitos não funcionais
- A Aplicação deve ser Modularizada:
    - Webpack 4

- Compatibilidade:
    - Babel

- Acessibilidade:
    - Utilizar tags HTML5 semânticas e com arial-attributes

- Versionamento de código:
    - Utilizar Git
    - Utilizar o serviço Github
    - Padronização de commits pelas ferramentas:
        - Commitlint
        - Commitizen
        - Husk

- Padronização de código:
    - Editor Config
    - ESLint
    - Prettier

- Tecnologias
    - Front-end
        - Utilizar ReactJs
        - Se necessário, usar React Redux ou a Context API do React para centralizar o estado
        - Utilizar Redux Saga para operações assíncronas
        - A interface deve usar funções com Debounce/Throttle (Principalmente na pesquisa)

- Deve ser totalmente Open Source
