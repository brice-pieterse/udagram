# Udagram

http://udagram-frontend-001.s3-website-us-east-1.amazonaws.com

This application is provided as a starter project for the purposes of learning to configure aws services, setting us a continuous integration/continuous deployment pipeline, and deploying an application. The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.

## Getting Started

1. Clone this repo locally into the location of your choice.
2. Open a terminal and navigate to the root of the repo
3. follow the instructions in the installation step

The project can run but is missing some information to connect to the database and storage service.

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres.
2. In AWS, provision a s3 bucket for hosting the uploaded files.
3. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/. The follow ENV variables should be add to your .env file:
    - POSTGRES_USERNAME
    - POSTGRES_PASSWORD
    - POSTGRES_DB
    - POSTGRES_HOST
    - DB_PORT
    - PORT (server)
    - URL (server)
    - JWT_SECRET
1. From the root of the repo, navigate into the udagram-api folder `cd udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal, navigate to the udagram-frontend `cd udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
2. `npm run test`
3. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
