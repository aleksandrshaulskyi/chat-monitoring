







# Chat-monitoring.

The monitoring microservice for the distributed chat system.

## Brief.

This microservice utilizes the modern and popular stack of  

**Opentelemetry** | **Prometheus** | **Grafana**  

to implement metrics monitoring. For the moment only vital metrics are monitored
such as the amount of the requests per second, latency for 95% and 99% of requests and
requests responded with an error.

## Stage.
This service is in the stage of active development. Updates are released multiple times a week.

## Features.
This microservice provides the monitoring solution for all of the microservices.

Comes with 3 provisioned dashboards for each of the backend microservices
of this project and the default Prometheus datasource.

Each dashboard contains the metrics that were listed above and the transportation
layer also contains the time series for the amount of the active connections to the
websocket hub.

## Usage.

1) Clone the repository.
2) Create the .env file using the example in the root directory.
3) Switch to the directory that contains the docker-compose file.
4) Run ```docker-compose up --build```.
5) That is it. Access Grafana on **http://localhost:3030**

## Recent updates.

None yet released.

## Back to Index repository of the whole chat system.

https://github.com/aleksandrshaulskyi/chat-index
