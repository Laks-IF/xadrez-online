## Xadrez Online
Plataforma com o principal objetivo de conectar jogadores de xadrez

### Requisitos Funcionais
- Gerenciar seu perfil 
    - Criar perfil
    - Atualizar perfil
    - Ver seu próprio perfil
    - Deletar perfil

- Sistema de ligação de contaas
    - Enviar/Receber pedidos de amizade
    - Aceitar/recusar pedidos de amizade
    - Ver pedidos de amizades recebidos/enviados pendentes
    - Cancelar pedidos enviados pendentes de amizade

- O jogador terá um perfil público
    - Contendo dados estatísticos
        - Quantidade de partidas jogadas
        - Quantidade de vitórias
        - Quantidade de derrotas
        - Quantidade de empates

    - Contendo dados públicos
        - Quantidade de amigos
        - Listagem de amigos

    - (OPCIONAL) Contendo dados de contato
        - Foto de perfil
        - Número de telefone
        - E-mail
        - Twitter
        - Facebook
        - Discord

- Sistema de procura por outros jogadores
    - Procurar pelo nickname único
    - Procurar pelo ID, também único
    - Pelo nome, porém não único

- Gerenciar salas
    - Criar salas
        - Com capacidade especificada

    - Deletar salas

    - Entrar/Sair de salas

    - Requisitos
        - Se a capacidade for maior que dois
        apenas dois jogadores jogam, o resto assiste
        - Em cada sala, deverá haver um chat

- Sistema de procura de salas
    - Pelo nome da sala
    - Pelo ID da sala
    - Filtrar pela quantidade minima/maxima de jogadores
    - Filtrar por salas cheias ou não


### Requisitos não funcionais
    
- Modularidade:
    - Webpack 4

- Compatibilidade:
    - Babel

- Acessibilidade :
    - Utilizar tags HTML5 semânticas e com arial-attributes

- Autenticação:
    - Usar no mínimo dois oAuth destas empresas:
        - Google
        - Facebook
        - Github
        - Gitlab
        - Microsoft

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