# Hosting a Full-Stack Application Udagram

## Description
 Udagram is an website application for posting picture from user to show it to the world.
 The application was provided from Udacity to be hosted in AWS with pipeline using CircleCi.
## URLS
- Backend URL: http://udagrambackend-env.eba-jsbbwkk3.us-east-1.elasticbeanstalk.com
- Frontend URL: http://udagram-bucket476684081341.s3-website-us-east-1.amazonaws.com

## Getting Started
Clone the project ```https://github.com/iSultanz/udacity-udagram.git``` then navigate to the root of the repository

To Run The project locally:
- To start Frontend:
    - navigate to the frontend folder - ```cd udagram/udagram-fronted```
    - install dependencies - ```yarn```
    - Start the frontend - ```yarn start```

- To start the backend:
    - navigate to the frontend folder - ```cd udagram/udagram-api```
    - install dependencies - ```npm install --force```
    - Setup .env file
    - Start the backend - ```npm run start:dev```

## Env
```
POSTGRES_USERNAME
POSTGRES_PASSWORD
POSTGRES_HOST
DB_PORT
PORT
POSTGRES_DB
AWS_SECRET_ACCESS_KEY
AWS_ACCESS_KEY_ID
AWS_BUCKET
AWS_REGION
AWS_REGION_DEFAULT
AWS_PROFILE
JWT_SECRET
URL
```

### Dependencies
```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version
- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project
- AWS CLI v2, v1 can work but was not tested for this project
- A RDS database running Postgres.
- A S3 bucket for hosting uploaded pictures.

```

## Deployment Steps:

- RDS database was used to create PostgresSQL for the application to store files
- S3 Bucket (image-container) for storing images from user
- S3 Bucket(Udagram-frontend) for hosting Frontend
- Elastic Beanstalk for hosting the APIs (Udagram-api)


## Built With And Deployed

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework
- [AWS](https://aws.amazon.com/) - Cloud Hosting Server

## License

[License](LICENSE.txt)
