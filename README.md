# ElasticStack images for ARM

This project aims to provide docker images that will run on ARM achitecture (like raspberry pi for example).

The docker images are built on a raspberry pi gitlab runner.

## Available apps

* Kibana v7.13.2
* ElasticSearch v7.13.2
* ElastAlert
* Elastic Indices Lifecyle : the [elastic-indices-lifecycle](https://gitlab.comwork.io/oss/elasticstack/elastic-indices-lifecycle)

# Git repositories

* main repo: https://gitlab.comwork.io/oss/elasticstack/elasticstack-arm
* github backup mirror: https://github.com/idrissneumann/elasticstack-arm
* gitlab backup mirror: https://gitlab.com/ineumann/elasticstack-arm

## Docker repositories

The images are available on docker hub:
* ElasticSearch: https://hub.docker.com/repository/docker/comworkio/elasticsearch
* Kibana: https://hub.docker.com/repository/docker/comworkio/kibana
* ElastAlert: https://hub.docker.com/r/comworkio/elastalert

Here's an example of docker-compose file to have an instance of ElasticSearch and Kibana on your raspberrypi: [here](./docker-compose-example.yml). You 

You also can pull the images directly with the tags below.

## Image tags

```shell
docker pull comworkio/elasticsearch:latest-arm
docker pull comworkio/elasticsearch:7.13.2-arm
docker pull comworkio/elasticsearch:7.13.2-1.1-arm
docker pull comworkio/elasticsearch:7.13.2-arm-{sha}
docker pull comworkio/elasticsearch:7.13.2-1.1-arm-{sha}
```

### Kibana

```shell
docker pull comworkio/kibana:latest-arm
docker pull comworkio/kibana:7.13.2-arm
docker pull comworkio/kibana:7.13.2-1.7-arm
docker pull comworkio/kibana:7.13.2-arm-{sha}
docker pull comworkio/kibana:7.13.2-1.7-arm-{sha}
```

### Elastalert

```shell
docker pull comworkio/elastalert:latest-arm
docker pull comworkio/elastalert:1.0-arm
docker pull comworkio/elastalert:1.0-arm-{sha}
```

