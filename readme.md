## Introduction
This is a Dockerfile to build a container image for rabbitmq

## Git repository
The source files for this project can be found here: https://github.com/taladocker/rabbitmq

## Pulling from Docker Hub
Pull the image from docker hub rather than downloading the git repo. This prevents you having to build the image on every docker host:

```
docker pull tala/rabbitmq
```

## Running
To simply run the container:

```
docker run -d --name talaria-rabbitmq -v /data/rabbitmq:/var/lib/rabbitmq tala/rabbitmq
```

### Management Plugin

```
docker run -d --name talaria-rabbitmq-management rabbitmq:3-management
```
