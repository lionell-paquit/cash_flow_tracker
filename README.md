# Dockerize Cash Flow Tracker App

> This project is created using the following technologies

| Technologies      |
|-------------------|
| React             |
| MongoDB           |
| NodeJS & Express  |
| Nginx             |
| Docker            |

## Prerequisite
* Docker needs to be installed on your machine

## Usage & Installation
The project can be installed using either of the following mechanisms:
* Copy the project in to your local machine  
  Use the "Clone or download" button and select "Download ZIP" to copy the entire project, and copy those into your project.
* Using git to clone
    ```sh
    git clone git://
    ```

## Using docker-compose file

In docker-compose-prod.yml change
```
MONGO_URI=${MONGO_URI}
```
I created mine on MongoDB Atlas if you want your database on the cloud.

## How to run the app

### Development
#### Building and running the app on development
```sh
docker-compose up -d
```
#### Stopping and removing the container on development
```sh
docker-compose down
```

### Production
#### Building and running the app on production
```sh
docker-compose -f docker-compose-prod.yml up -d
```
#### Stopping and removing the container on production
```sh
docker-compose -f docker-compose-prod.yml down
```

## Future learning
* To be able learn how to manage the container and deploy it using Kubernetes
* How to add self-healing metrics
* How to add support for metrics and request tracking