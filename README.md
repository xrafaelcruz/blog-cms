##### pt-br

# Blog CMS

Criado com [`Strapi`](https://strapi.io/documentation/developer-docs/latest/getting-started/quick-start.html#_1-install-strapi-and-create-a-new-project).

Esse projeto contém o CMS/API para o meu blog.

## Requisitos

- node.js
- yarn
- postgres

#### Comandos

- `develop`: Executa a aplicaçáo em modo de desenvolvimento
- `build`: Cria o build para deploy
- `start`: Executa o projeto em cima do build
- `strapi`: CLI, utilizado para os comandos anteriores

## Start

### .env

Gerar a partir do .env.example e preencher os valores necessarios.

### Postgres

Caso nao tenha o postgres, executar:

```
docker-compose up
```

Ele ira buscar as variaveis preenchidas anteriormente no .env para criar um container do postgres.

### App

Instalar as dependencias

```
yarn
```

Executar o modo de desenvolvimento

```
yarn develop
```
