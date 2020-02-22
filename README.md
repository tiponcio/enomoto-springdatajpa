# Spring Data JPA
This project shows how to use Spring Data JPA using MySQL or Oracle

## MySQL
* `docker run --name poc-mysql -e MYSQL_ROOT_PASSWORD=123456 -d -p 3306:3306 mysql:5.7`
* `docker exec -it poc-mysql bash`
* `mysql -u root -p 123456`
* `create database db_example`
* `create user 'springuser'@'%' identified by 'ThePassword';`
* `grant all on db_example.* to 'springuser'@'%';`
* `exit`
* `mvn spring-boot:run`

## Oracle
* `https://github.com/wnameless/docker-oracle-xe-11g`
* `docker run -d -p 49161:1521 -p 8080:8080 wnameless/oracle-xe-11g-r2`

hostname: localhost
port: 49161
sid: xe
username: system
password: oracle
