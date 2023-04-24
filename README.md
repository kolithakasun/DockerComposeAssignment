# Devops-Assignment

This repo contains the solution for the below technical evaluation.

*Technical Evaluation*
```
Create three Docker containers, on your PC as below.
One docker container that runs a simple "hello world" application.
The second that runs Nginx or Apache to expose the above docker application.
The third one, runs a database (you can choose any database of your choice).
Send us the bitbucket / GitHub repository that contains a docker-compose file and three Docker files (one per app) and the docker-compose must start this Hello World application.
```

All 3 Dockerfiles are within the respective directory.

# App

sample Python Flask application is listning on port 5000. it can be access via nginx.

Links: https://localhost:80/, https://localhost:80/app

# Connecting to the Database

The Database root password is stored in a seperate file named `.env`. I have uploaded it to this repo as example, otherwise we can skip it using `.gitignore`. Please store it as below.

```
MYSQL_ROOT_PASSWORD=rootpasswordthatyouneed
```

To connect to mysql database, follow below command. *you need to install mysql client*
```
mysql -u root -p -h 127.0.0.1 -P 3306
```

# Start using docker-compose

Use the below command to start docker containers.

```
docker-compose up
```

To start docker-compose in Detached mode

```
docker-compose up -d
```