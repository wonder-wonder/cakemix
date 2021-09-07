# Example for deploying cakemix
This is a example for cakemix deploy.

## How to run
This example use `docker` and `docker-compose`. Please make sure they can be used.  
Then just do `docker-compose up` in the directory. You can access [`http://localhost:8081/`](http://localhost:8081/)  

The default username is `root` and password is `cakemix`. **Please change the password firstly.**  

## docker-compose.yml
Cakemix needs API server and DB server. `docker-compose` is best way to run both containers.  
Please see [docker-compose.yml](docker-compose.yml) in detail.  
Please be careful of server and DB data location. (This example use docker volume to preserve data. You can also consider to use bind mount.)

## initdb
The directory contains the SQL commands for DB initalization.
The directory is same as [cakemix-server/docker/postgres/init](https://github.com/wonder-wonder/cakemix-server/tree/main/docker/postgres/init).