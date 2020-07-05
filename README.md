# Employee System

I created an Employee System application for handling the data of employees.

## Install the Application

To run the application in development, you have to use `docker-compose` to run the app with `docker`:

```bash
docker-compose up -d
```

Run this command from CLI mode of the docker-webserver container from the directory in which you want to install the application.

```bash
composer install
```

## Import employees database
Run these command from CLI mode of the docker-mysql container

```bash
cd /tmp/database

mysql -u root -p
The password will be asked: type securedPassw0rd

source employees.sql
```

## Run
 unit tests

Run this command from CLI mode of the docker-alpine container to run the unit tests.

```bash
composer test
```

## Run unit tests and show code coverage

Run this command from CLI mode of the docker-alpine container to run the unit tests with code coverage displaying.

```bash
composer display-coverage
```

## Run unit tests and write code coverage to html

Run this command from CLI mode of the docker-alpine container to run the unit tests and write code coverage to html.

```bash
composer html-coverage
```

## Usage

## Possible improvements