## Xadrez Online
Plataforma com o principal objetivo de conectar jogadores de xadrez

### Requisitos Funcionais
1. __Gerenciar seu perfil:__
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

2. __Sistema de amigos:__
    - Enviar/Receber pedidos de amizade
    - Aceitar/recusar pedidos de amizade
    - Ver pedidos de amizades recebidos/enviados pendentes
    - Cancelar pedidos de amizade enviados e que pendentes

3. __O jogador terá um perfil público:__
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

4. __Sistema de busca:__
    - Por outros jogadores
        - Procurar pelo nickname único
        - Procurar pela tag, também único
        - Pelo nome, porém não único
    - Por jogos
        - Pelo nome do jogos
        - Pela tag do jogo

5. __Gerenciar jogos:__
    - Criar jogos
        - Definir como público (Qualquer jogador pode entrar no jogo criado) ou privado (O jogo não será listado na busca de jogos, outro jogador só poderá entrar no jogo com o link de convite)
        - Desafiar outro jogador diretamente pelo perfil
        - Poder aceitar/recusar jogos
    - Assistir jogos
        - Possibilidade assistir jogos públicos acontecendo no momento

7. __Gerenciar partidas dentro das salas:__
    - Quando estiver em uma sala de xadrez como telespectador, é possível usar o chat
    - Quando estiver em uma sala de xadrez como jogador, há somente o tabuleiro, sem chat
    - Ao fim de cada partida
        - Os dados devem ser contabilizados para o perfil e os dois jogadores devem ser redirecionados para a página

9. __A aplicação deve ter tema Escuro e Claro__

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