## Xadrez Online
Plataforma com o principal objetivo de conectar jogadores de xadrez

### Requisitos Funcionais
- Gerenciar seu perfil 
    - Operações (CRUD)
        - Criar perfil
        - Atualizar perfil
        - Ver seu próprio perfil
        - Deletar perfil
    - Sessão
        - Sair do perfil
        - Entrar novamente no perfil
    - Forma de criar perfil
        - O jogador pode fazer login no perfil ou criar um a partir de uma rede social

- Sistema de amigos
    - Enviar/Receber pedidos de amizade
    - Aceitar/recusar pedidos de amizade
    - Ver pedidos de amizades recebidos/enviados pendentes
    - Cancelar pedidos de amizade enviados e que pendentes

- O jogador terá um perfil público
    - Contendo dados estatísticos
        - Quantidade de partidas jogadas
        - Quantidade de vitórias
        - Quantidade de derrotas
        - Quantidade de empates
    - Contendo dados públicos
        - Quando se registrou na plataforma
        - Quantidade de amigos
        - Listagem de amigos
    - (OPCIONAL) Contendo dados de contato
        - Foto de perfil
        - Número de telefone
        - E-mail
        - Twitter
        - Facebook
        - Discord

- Sistema de procura
    - Por outros jogadores
        - Procurar pelo nickname único
        - Procurar pela tag, também único
        - Pelo nome, porém não único
    - Procura de salas
        - Pelo nome da sala
        - Pela tag da sala
        - Filtrar pela quantidade minima/maxima de jogadores
        - Filtrar por salas cheias ou não

- Gerenciar salas
    - Criar salas
        - Com capacidade especificada, com no máximo 10 pessoas
    - Deletar salas
    - Entrar/Sair de salas
    - Requisitos
        - Em cada sala, deverá haver um chat

- Gerenciar partidas dentro das salas:
    - Poderá desafiar outro jogador ou receber desafios para uma partida
    - Possibilidade de aceitar/recusar desafios
    - Ao aceitar, os dois irão para uma página com um tabuleiro de xadrez
    - Ao acabar a partida, os dados devem ser contabilizados para o perfil e os dois jogadores devem ser redirecionados para a mesma sala, se houver

- Sistema de 


### Requisitos não funcionais
    
- A Aplicação deve Modularizada:
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
    - Usar Token JWT para autenticação

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
        - A interface deve user funções com Debounce (Pesquisa)

    - Back-end
        - Servidor em NodeJs
        - Utilizando o Framework Express.js ou Adonis.js
        - Real Time: Protocolo Websocket com algum destes:
            - Socket.io
            - Feathers
            
    - Banco de dados:
        - Banco de dados não relacional MongoDB
        - ORM Mongoose ou Sequelize

- Deve ser totalmente Open Source