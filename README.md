# Introduction

This repository provides the OPAL demonstrator, consisting of the [Web UI](https://github.com/projekt-opal/web-ui) and [Webservices](https://github.com/projekt-opal/opal-webservices). 


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
you have the demo containers running and the demo is available on port 3000 (you can set any port that you want in the docker-compose.yml) of your server.


## Credits

[Data Science Group (DICE)](https://dice-research.org/) at [Paderborn University](https://www.uni-paderborn.de/)

This work has been supported by the German Federal Ministry of Transport and Digital Infrastructure (BMVI) in the project [Open Data Portal Germany (OPAL)](http://projekt-opal.de/) (funding code 19F2028A).
