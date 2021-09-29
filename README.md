# Mongodb BI Connector

this docker image for mongodb-bi-connector.

## docker-compose example

```
version: "3.8"

services:
  mongodb:
    image: mongo:bionic

  mongodb-bi-connector:
    image: chuntungho/mongodb-bi-connector
    ports:
      - 3307:3307
    volumes:
      - ./mongosqld-config.yml:/mongosqld/mongosqld-config.yml
```
