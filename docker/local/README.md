# Local development stack

## Supporting services

|Port | Service | Connection |
|---|---|---|
| 27017 | MongoDB | mongodb://root:passwd@localhost:27017 |
| 5432 | PostgreSQL | jdbc:postgresql://postgres:changeme@localhost:5432 |
| | RabbitMQ |  e.g.: amqp://guest:guest@localhost:5672 |
|1883| MQTT-Broker |tcp://user:passwd@localhost:1883 |
| | Consul | spring auto configuration |

## Management Tools

| Service | Authentification |
|---|---|
| [Consul ](http://localhost:8500) | no authentication needed |
| [Mongodb](http://localhost:8081/db/test/) | no authentication needed |
| [RabbitMQ](http://localhost:15672/) | user: guest / password: guest |

## Enabled features in RabbitMQ

| Port | Feature/Documentation |
|---|---|
| 5672 | [RabbitMQ: Advanced Message Queuing Protocol) (AMQP)](https://www.rabbitmq.com/tutorials/amqp-concepts.html) |
| 1884 | [RabbitMQ: Message Queuing Telemetry Transport (MQTT) 3.1.1](https://www.rabbitmq.com/mqtt.html) |
| 61613 | [RabbitMQ: Simple (or Streaming) Text Orientated Messaging Protocol (STOMP)](https://www.rabbitmq.com/stomp.html) |
| 15675 | [RabbitMQ: Message Queuing Telemetry Transport (MQTT) 3.1.1 over Websocket](https://www.rabbitmq.com/web-mqtt.html) |

## Consul

[Feign clients](../../feign-support/README.md) Service discovery for local development

| Port | Purpose |
|---|---|
| 8300 | server: Server RPC address |
| 8500 | HTTP: The HTTP API |
| 8600 | DNS: The DNS server |
