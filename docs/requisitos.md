## Xadrez Online
Plataforma com o principal objetivo de conectar jogadores de xadrez

### Requisitos Funcionais
- Gerenciar Playlists:
  - Poder criar uma nova Playlist
  - Poder deletar uma Playlist existente
  - Poder adicionar músicas à Playlist existente
  - Poder ouvir Playlists
  
- Gerenciar músicas
  - Poder salvar uma música em uma das Playlists
  - Poder remover uma música de uma Playlist
  
- Download de músicas
  - Poder fazer o Download de uma música
  - Poder fazer Download de uma Playlist
  - Poder fazer Download de um arquivo CSV com os dados de uma Playlists e suas músicas
  
- Aba de configurações
  - Possibilidade de trocar temas
  - Deve ter a opção de alternar temas além do Light e Dark
  - Possibilidade de alterar a tipografia (fonte)
  
### Requisitos não funcionais
- A Aplicação deve ser Modularizada:
    - Webpack 4

- Compatibilidade:
    - Babel

- Acessibilidade:
    - Utilizar tags HTML5 semânticas e com arial-attributes

- Autenticação:
    - Usar no mínimo dois oAuth destas redes sociais:
        - Google
        - Facebook
        - Github
        - Gitlab
        - Microsoft
    - Gerar Token JWT para autenticação

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
        - Se necessário, usar React Redux para centralizar o estado
        - Utilizar Redux Saga para operações assíncronas
        - A interface deve usar funções com Debounce/Throttle (Principalmente na pesquisa)

    - Back-end
        - Servidor em NodeJs
        - Utilizando o Framework Express.js ou Adonis.js
        - Real Time: Protocolo Websocket com algum destes:
            - Socket.io
            - Feathers
            
    - Banco de dados:
        - Banco de dados não relacional MongoDB
        - ORM Mongoose

- Deve ser totalmente Open Source
