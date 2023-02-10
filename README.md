# Project Management Tool with React / Next.js

A project management app built with Next.js while going through the Frontend Masters course "[Build a Fullstack App with Next.js, v2](https://frontendmasters.com/courses/fullstack-app-next-v2/)" from Scott Moss.

## Getting started

### Add .env file

- Create the file `.env` in the root of the project
- Add the following environment variables in a VARIABLE=VALUE manner to the file

| VARIABLE     | EXAMPLE VALUE                                                                            | DESCRIPTION                                     |
| ------------ | ---------------------------------------------------------------------------------------- | ----------------------------------------------- |
| DATABASE_URL | postgresql://pmfmuser:pmfmpass@localhost:5433/project-management-nextjs-fm?schema=public | Connection string for the PostgreSQL database\* |

\* "Example Value" can be used as is for the docker environment provided in this project

### Run docker environment

The following command will run all necessary services specified in the `docker-compose.yml` file:

```bash
docker-compose up
```

### Push database migrations

Apply the Prisma database migrations to the database by running:

```bash
npm run db:push
```

### Push database data

```bash
npm run db:seed
```

### Run app

```bash
npm run dev
```
