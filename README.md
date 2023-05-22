# Oportunities 

Este projeto é uma API moderna de oportunidades de trabalho construída usando Golang. A API é alimentada por Go-Gin como roteador, GoORM para comunicação de banco de dados, SQLite como banco de dados e Swagger para documentação e teste de API. O projeto segue uma estrutura de pacotes moderna para manter a base de código organizada e de fácil manutenção. 

## Features

- Configuração do ambiente de desenvolvimento para criação da API
- Usando o Go-Gin como roteador para gerenciamento de rotas
- Implementação do SQLite como banco de dados para a API
- Usando GoORM para comunicação com o banco de dados
- Integração do Swagger para documentação e teste de API
- Criação de uma estrutura de pacotes moderna para organização do projeto
- Implementação de uma API completa de oportunidades de emprego com endpoints para pesquisar, criar, editar e excluir oportunidades
- Implementação de testes automatizados para garantir a qualidade da API

## Dependencies

Para usar este projeto, você precisa seguir estas etapas:

1. Clone o repositório: `git clone https://github.com/username/repo-name.git`
2. Instale as dependências: `go mod download`
3. Crie o aplicativo: `go build`
4. Execute o aplicativo: `./main`

## Makefiles Commands

O projeto inclui um Makefile para ajudá-lo a gerenciar tarefas comuns com mais facilidade. Aqui está uma lista dos comandos disponíveis e uma breve descrição do que eles fazem:

- `make run`: Executa a aplicação sem gerar a documentação da API.
- `make run-with-docs`: Gere a documentação da API usando o Swag e execute o aplicativo.
- `make build`: Compile o aplicativo e crie um arquivo executável chamado `gopportunities`.
- `make test`: Executa testes para todos os pacotes do projeto.
- `make docs`: Gera a documentação da API usando Swag.
- `make clean`: Remova o executável `gopportunities` e exclua o diretório `./docs`.

Para usar esses comandos, basta digitar `make` seguido do comando desejado em seu terminal. Por exemplo:

```sh
make run
```

## Docker and Docker Compose

Este projeto inclui um arquivo `Dockerfile` e `docker-compose.yml` para fácil conteinerização e implantação. Aqui estão os comandos mais comuns do Docker e do Docker Compose que você pode querer usar:

- `docker build -t your-image-name .`: Constrói uma imagem do Docker para o projeto. Substitua `your-image-name` por um nome para sua imagem.
- `docker run -p 8080:8080 -e PORT=8080 your-image-name`: Executa um contêiner com base na imagem construída. Substitua `your-image-name` pelo nome que você usou ao construir a imagem. Você pode alterar o número da porta, se necessário.

Se você quiser usar o Docker Compose, siga estes comandos:

- `docker compose build`: Constrói os serviços definidos no arquivo `docker-compose.yml`.
- `docker compose up`: Executa os serviços definidos no arquivo `docker-compose.yml`.

Para parar e remover contêineres, redes e volumes definidos no arquivo `docker-compose.yml`, execute:

```sh
docker-compose down
```

