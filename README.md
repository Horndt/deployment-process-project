# Hosting a Full-Stack Application

## Desciption

The final Project from Udacity is provided to be hosted into AWS with Pipeline using CircleCI.

### Dependencies

```
- Node v14.15.1 (LTS) or more recent

- npm 6.14.8 (LTS) or more recent

- AWS CLI v2, v1 can work but was not tested for this project

- RDS database running Postgres.

- S3 bucket for hosting uploaded pictures.

```

## Getting Started

### install

- clone this repo 'https://github.com/Horndt/deployment-process-project.git'
- navigate in your terminal to the root directory
- run
  - `npm run frontend:intall` to install frontend dependencies
  - `npm run api:install` to install backend dependencies

### build

- run
  - `npm run frontend:build` to build the frontend
  - `npm run api:build` to build the backend

## Test

1. `cd udagram/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no tests on the back-end

## Deploy

### manually

- frontend: in root run `npm run frontend:deploy`
- backend: in root run `npm run api:deploy`

### automated

- Push new commits to repo. This triggers the pipeline to start the deployment process.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
