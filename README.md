# Dockerized ESRI Geoportal Catalog Server and Harvester 

Kartoza Fork from https://github.com/ma-ku/docker-geoportal.git

This project bundles all prerequisites needed to run the geoportal server and a harvester are captured in this docker composition. The docker-compose.yml creates two containers, one running Tomcat with the [geoportal-server-catalog](https://github.com/Esri/geoportal-server-catalog) and the [geoportal-harvester](https://github.com/Esri/geoportal-harvester). The second container provides the Elasticsearch server for storing and indexing the data stored in the catalog server.

## Releases and Downloads
- Version 2.5.0 of geoportal-server-catalog and geoportal-harvester.

## Installation
 
Clone the repository to your local drive. In order to build the containers and run them, use the following commands:
```bash
$ git clone https://github.com/kartoza/docker-geoportal.git
$ cd docker-geoportal/src
$ docker network create geoportal
$ docker-compose build
$ docker-compose up
```

## Run the applications

* Connect to http://localhost:8080/geoportal to see the geoportal in action. 
* Connect to http://localhost:8080/harvester to see the harvester in action. 

## Requirements

* Docker

