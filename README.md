# Nest Clean

## 💻 Projeto

**[Nest Clean](https://github.com/AdrianoTobias/nest-clean)**, é uma aplicação com o framework NestJS, voltada ao desenvolvimento de serviços Web para um "Fórum", o qual engloba API's REST de criação, leitura, atualização e deleção de perguntas, respostas e comentários, além de tratativas com anexos (watched list) e de eventos de notificações (subscriber). O projeto segue a modelagem "Domain Driven Design (DDD)" e o conceito de "Clean Architecture", inclusive, sua camada de domínio é a do projeto [Node Clean-DDD](https://github.com/AdrianoTobias/node-clean-ddd).

O projeto possui, ainda, autenticação e controle de acesso a rotas, bem como a implementação de cache, testes (unitários e end-to-end) e integração com o [Cloudflare](https://www.cloudflare.com/).

É uma aplicação desenvolvida durante o **[MBA Fullstack](https://www.rocketseat.com.br/mba)**, provido pela **[Rocketseat](https://rocketseat.com.br/)**, em parceria com a **[Sirius Education](https://landing.sirius.education/home/)**.


## 🧪 Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:

- [NestJS](https://docs.nestjs.com/)
- [TypeScript](https://www.typescriptlang.org/)
- [Prisma](https://www.prisma.io/)
- [Redis](https://redis.io/)
- [Zod](https://github.com/colinhacks/zod)
- [Vitest](https://vitest.dev/)


## 🚀 Como executar

Clonar o projeto e acessar a pasta do mesmo:

```bash
$ git clone https://github.com/AdrianoTobias/nest-clean.git
$ cd nest-clean
```

Para iniciá-lo:
```bash
# Instalar as dependências
$ npm install
```

> Esse projeto depende do [Docker](https://docs.docker.com/get-started/get-docker/) para rodar os bancos de dados. Após tê-lo instalado:

```bash
# Criar o container
$ docker compose up -d

# Criar a estrutura dos bancos de dados (aplicação e Redis)
$ npx prisma migrate dev
```

```bash
# Iniciar a aplicação
$ npm run start:dev
```
A aplicação estará disponível no endereço http://localhost:3333 e o Redis no endereço http://localhost:6379.

Para executar os testes:
```bash
# Iniciar os testes unitários
$ npm run test

# Iniciar os testes end-to-end
$ npm run test:e2e
```



[Adriano Tobias](https://github.com/AdrianoTobias)