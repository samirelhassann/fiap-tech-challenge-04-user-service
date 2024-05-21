# FIAP SOAT - Grupo 65 - Tech Challenge #04 - Application

Repositório do Tech Challenge #04 da FIAP/Alura, no curso SOAT3. 

Este projeto é uma evolução do projeto do Tech Challenge #03.

## Como rodar a aplicação?

### Rodando Localmente

Pré-requisitos:

- [Node.js](https://nodejs.org/en) `>= 18.x`
- [Yarn](https://yarnpkg.com/) - versão usada localmente: `1.22.21`
- [Docker](https://www.docker.com/) - versão usada localmente: `4.27.2`

Após se certificado dos pré requisitos, siga o seguinte passo a passo:

1. Rode o docker compose para subir o banco de dados postgres
```bash
docker-compose up -d
```

2. Instale as dependências do projeto
```bash
yarn install
```

3. Atualize o prisma e subida das tabelas no banco de dados via migration
```bash
yarn prisma generate && yarn prisma migrate dev
```

4. Inicialize a aplicação
```bash
yarn dev
```

A aplicação estará disponível, por padrão, na rota [`http://localhost:3001`](http://localhost:3001).

# Documentação (API)

Ao rodar o projeto é possível acessar com o endpoint `/docs` a documentação completa no [Redoc](https://github.com/Redocly/redoc) ou em `/docs-swagger` para a visualização do [Swagger](swagger.io) padrão.

## Membros
- [Samir El Hassan](github.com/samirelhassann)
