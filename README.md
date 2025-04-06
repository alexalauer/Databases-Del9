# Project Deliverable 9 - template

This report supports project deliverable 9.  Deliverable 9 is all about project acceleration -
we're focusing on kickstarting development of your database and web application.

## Tasks

For this assignment I explored five different docker examples and prepared
a report summarizing my activities.


A docker tutorial is here: <https://vcu-ssg.github.io/ssg-quarto-docker-tutorial/>


## Examples

The repo contains a bunch of docker examples, as listed below.  These links take you 
directly to the GITHUB repo and the respective README files.

The `README.md` files in each folder provide background on the example and provide instructions for running each example.  The first two examples use `docker` commands while the last three use `docker-compose`.  

* [nginx-static-example](https://github.com/vcu-ssg/ssg-quarto-docker-tutorial/tree/main/site/example-nginx-static-example) - creates a simple, static web server with the html file stored inside the container.

* [nginx-static-volume](https://github.com/vcu-ssg/ssg-quarto-docker-tutorial/tree/main/site/example-nginx-static-volume) - creates a simple web server container with the html files stored on your local disk.

* [apache-php-remote-mysql](https://github.com/vcu-ssg/ssg-quarto-docker-tutorial/tree/main/site/example-apache-php-remote-mysql) - creates a local apache web server serving html/php pages from your local disk, connected to cmsc508.com using your username and password.

* [apache-php-local-mysql](https://github.com/vcu-ssg/ssg-quarto-docker-tutorial/tree/main/site/example-apache-php-local-mysql) - creates a local apache setb server serving html/php pages from your local disk, connected to a locally running mysql DB and locally running phpmyadmin.

* [production-example-1](https://github.com/vcu-ssg/ssg-quarto-docker-tutorial/tree/main/site/example-production-example-1) - creates a localling running nginx load balancer and reverse proxy, apache-php server, mysql database and phpmyadmin all talking together.

## Installation and Setup

### Prerequisites
- [Docker](https://www.docker.com/)

### Cloning the Repository
```bash
git clone https://github.com/your-username/example-nginx-static-example.git
cd example-nginx-static-example
```

### Building and Running with Docker 
```bash
docker build -t example-nginx-static-examplep .
docker run -d -p 8080:80 example-nginx-static-example
```

### Accessing the Application 
Visit http://localhost