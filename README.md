# gost service

The `GOST` service provides an [OGC SensorThings API](http://www.opengeospatial.org/standards/sensorthings) (STA) REST service based
on [Geodan GOST Server](https://github.com/gost/server).

## Hosting

The Docker Image is hosted as: [smartemission/se-gost at DockerHub](https://hub.docker.com/r/smartemission/se-gost).

## Environment

The following environment vars need to be set, either via `docker-compose` or
Kubernetes.

|Environment variable|
|---|
|GOST_SERVER_EXTERNAL_URI|
|GOST_DB_HOST|
|GOST_DB_PORT|
|GOST_DB_DATABASE|
|GOST_DB_USER|
|GOST_DB_PASSWORD|

## Architecture

The image includes the official Geodan GOST Server Docker Image overlayed with
the SE config file. Further vars from that config are overrruled/set via its 
Container Environment at runtime. 

## Links

* SE Platform doc: http://smartplatform.readthedocs.io/en/latest/
* OGC SensorThings API Standard: http://www.opengeospatial.org/standards/sensorthings
