# Introduction

This is  a demo project for the opal webui and opal webservices. 

# How to run

To be able to run you must provide a .env file in the root folder of the project that is similar to
```
BACKEND_ADDRESS=http://localhost:8081/
OPAL_TRIPLESTORE_URL=localhost
OPAL_TRIPLESTORE_USERNAME=xxxx
OPAL_TRIPLESTORE_PASSWORD=xxxx
```
Then, by running the command 
```
docker-compose up -d
```
You have the demo containers running and it is available on the port 3000 (you can set any port that you want in the docker-compose.yml) of your server.
