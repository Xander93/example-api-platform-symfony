# example-api-apiplatform :tada:
This is a REST API Example based on Symfony and API Platform.

## Requirements :package:
- Composer
- PHP x.x CLI
- Docker
- Docker-compose

## Setup 🔨
- Clone the project with git  
`git clone https://github.com/Xander93/example-api-apiplatform.git <project-dir>`

- Run composer in the project directory to install all the dependencies.  
`composer install`

- Run docker compose to start all the required containers.  
`docker compose up -d`

- Now the REST API Example should be running on:  
`http://localhost:80`

- To get our API working we have to create our database and our tables with the following commands:  
`docker-compose exec fpm ./bin/console doctrine:database:create`  
`docker-compose exec fpm ./bin/console doctrine:schema:create`

## API Documentation :memo:
The API documentation can be found in the above mentioned url or click here: <br>
http://localhost/docs?ui=re_doc

## This repo is making use of Dependabot 🤖
- Automated dependency updates built into GitHub
