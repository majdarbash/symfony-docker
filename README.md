

Table of Contents
=================
- [Installation] (#installation)
- [FAQ] (#faq)

## Installation

> Build and run the containers:
```
APP_PATH=$PWD COMPOSER_HOME=$(realpath ~/)"/.composer" bash -c 'docker-compose up -d --build'
```
> Create the database:
```
docker exec -it symfony-docker_db_1 mysql -uroot -proot -e 'create database symfony'
```
> Check database was created successfully:
```
docker exec -it symfony-docker_db_1 mysql -uroot -proot -e 'show databases'
```