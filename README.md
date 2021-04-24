##### pt-br

# Blog CMS

Criado com [`Strapi`](https://strapi.io/documentation/developer-docs/latest/getting-started/quick-start.html#_1-install-strapi-and-create-a-new-project).

Esse projeto contém o CMS/API para o meu blog.

## Requisitos

- node.js
- yarn
- postgres

#### Comandos

- `develop`: Executa a aplicaçáo em modo de desenvolvimento com autoreload
- `build`: Constroi o painel administrativo
- `start`: Executa o projeto em modo de produção com autoreload desabilitado
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

Construir a aplicacao

```
yarn build
```

Executar o modo de desenvolvimento com autoreload

```
yarn develop
```
