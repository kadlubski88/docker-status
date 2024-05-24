# Description
A simple tool to inspect the status of your docker engine and containers as plain text or as json

## Usage
docker-status [OPTIONS]

## options
- --json <br> output as a json

## Ouput example
plain text:
~~~
Docker engine
-------------
Version:        Docker version 24.0.5, build 24.0.5-0ubuntu1~22.04.1

Containers
----------
Total:          4
Running:        1
   Healthy:        0
   Unhealthy:      0
   Undefined:      1
Exited:         2
Paused:         1

Images
------
Total:          1
Size:           7.79 MB
~~~
json
~~~
{"container_total":2,"container_running":0,"container_exited":1,"container_paused":1,"container_health_healthy":0,"container_health_unhealthy":0,"container_health_undefined":2,"image_total":1,"image_size":7794716}
~~~
