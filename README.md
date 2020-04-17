# node-structure

## Aplicação em node para API REST com:
  - modelo de estrutura de pasta/arquivos
  - express
  - ORM (sequelize)
  - CRUD Exemplo utilizando o postgres
  - testes de integração de Exemplo utilizando o sqlite
  - docker-compose subindo postgres + pgAdmin
  
 ## Pré-requisitos (instalações)
  - node
  - yarn
  - docker e docker-compose
   
 ## Rodando aplicação
  - criar arquivo .env e preencher as variaveis de embiente (dica: ctrl+C e ctrl+V do arquivo .env.example)
  - rodar no teminal (na raiz do projeto) os comandos abaixo:  
    ```
      yarn 
      docker-compose up -d
      yarn sequelize db:migrate
      yarn dev
    ```
    Descrição dos comandos acima:
      - yarn (instalar as dependencias da aplicação caso necessário)
      - docker-compose up -d (subir o postgres + pgAdmin)
      - yarn sequelize db:migrate (criar as tabelas no banco de dados)
      - yarn dev (iniciar a aplicação com nodemon em http://localhost:3333)
    
    ## Rodando testes
  - criar arquivo .env.test e preencher as variaveis de embiente (dica: ctrl+C e ctrl+V do arquivo .env.test.example)
  - rodar no teminal (na raiz do projeto) os comandos abaixo:  
    ```
      yarn
      yarn test
    ```
    Descrição dos comandos acima:
      - yarn (instalar as dependencias da aplicação caso necessário)
      - yarn test (para rodar os testes criados dentro do diretório __tests__)
