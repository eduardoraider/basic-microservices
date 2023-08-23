# Basic Microservices Architecture

Microservices architecture (often shortened to microservices) refers to an architectural style for developing applications. Microservices allow a large application to be separated into smaller independent parts, with each part having its own realm of responsibility. To serve a single user request, a microservices-based application can call on many internal microservices to compose its response.

## Project Setup

1. Clone the repository: `git clone --recursive https://github.com/eduardoraider/basic-microservices.git`
2. Navigate to the project directory: `cd basic-microservices`
3. Follow the steps below. 

## Build and Run

>_**NOTE**_: You will need to set up a gmail account to send email. To do so, define in `docker-compose.yml` the variables `GMAIL_USER` and `GMAIL_PASSWORD` with the correct values.

This command will build the containers and then start the project in detached mode.
```bash
docker-compose up -d --build
```
Start and Stop a Docker Compose Project.
Start:
```bash
docker-compose up -d
```
Stop:
```bash
docker-compose down
```

## Local URLs - API Gateway
| URLs                           |
| :----------------------------- |
| http://localhost:4200/login    | 
| http://localhost:4200/compra   |
| http://localhost:4200/cursos   | 
| http://localhost/mkt/leads     |

## Submodules
| Repository          |  Description                                  |
| :------------------ |:----------------------------------------------|
| academico-php       |  Microservice that consumes queues using PHP  |
| academico-php-web   |  API of academico-php Microservice            |
| financeiro-php      |  Microservice for API and background jobs     |
| front-end           |  Microservice with frontend.                  |
| mkt-node            |  Microservice for marketing containing both the API and the queue consumer. |

## Container Names
| Container Name       |
| :------------------- |
| front                | 
| web-mkt              |
| mongo-mkt            |
| rabbitmq             | 
| web-financeiro       | 
| api-gateway          | 
| consumer-academico   | 
| postgre-academico    | 
| web-academico        | 


#### 🛠 by Eduardo O Raider
**Software Engineer**