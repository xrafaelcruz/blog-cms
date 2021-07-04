##### pt-br

# Blog CMS

Criado com [`Strapi`](https://strapi.io/documentation/developer-docs/latest/getting-started/quick-start.html#_1-install-strapi-and-create-a-new-project).

Esse projeto contém o CMS/API para esse [blog](https://gitlab.com/xrafaelcruz/blog-frontend).

## Requisitos

- node.js
- yarn
- postgres

## Start

#### .env

Criar o arquivo .env a partir do .env.example e preencher os valores necessarios.

#### Postgres

Caso nao tenha o postgres, é possível utiliza-lo com o docker.

Para isso é necessário estar rodando o docker na máquina e executar o comando na raiz do projeto:

```
docker-compose up
```

Ele ira buscar as variaveis preenchidas anteriormente no .env para criar um container do postgres.

O passo a passo gera o resultado a baixo

- preenchimento do .env
- execução do comando docker-compose up

Foi utilizado o dbeaver para validar a conexão com o banco.

![Alt text](/assets/docker-postgres.png?raw=true "Resultado após executar docker-compose up")

#### App

Instalar as dependencias

```
yarn
```

Construir a aplicacao (mesmo para rodar apenas o modo de desenvolvimento)

```
yarn build
```

Executar o projeto primeiramente dessa maneira

```
yarn start
```

Criar o cadastro e logar, após esses passos é possível executar o modo dev.

Foi detectado alguns bugs ao executar a primeira vez com o comando **dev** e por isso esse processo.

**Liberar o acesso publico para as consultas na API**

![Alt text](/assets/access.png?raw=true "Resultado após executar docker-compose up")

## Comandos

- `dev`: Executa a aplicaçáo em modo de desenvolvimento com autoreload
- `build`: Constroi o painel administrativo
- `start`: Executa o projeto em modo de produção com autoreload desabilitado
- `strapi`: CLI, utilizado para os comandos anteriores
