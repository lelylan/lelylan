# Lelylan: Open Source Internet of Things

Lelylan is an iot cloud platform based on a lightweight microservices architecture.

Lelylan platform is both hardware-agnostic and platform-agnostic. This means you can connect any hardware, from the ESP8622 to the most professional embedded hardware solution and everything in between - and it can run on any public cloud or in your own private datacenter, or even a hybrid environment, whether virtualized or on bare metal.

![Lelylan Logo](https://raw.githubusercontent.com/lelylan/lelylan/master/public/logo-lelylan.png)

### Why Lelylan

Research in the Internet of Things is global and growing fast, but lacks standard tools. Many companies are building their own solution. By sharing what we have learned during the years, we want to create a shared code base for the Internet of Things. To see Lelylan in action checkout the [tuturials](http://dev.lelylan.com/#overview-tutorials) in the dev center. 

### Resources

* [Architecture](http://dev.lelylan.com/architecture) (how Lelylan works)
* [API](http://dev.lelylan.com/api) (how to use Lelylan)
* [Blog](http://lelylan.com) (latest from Lelylan)



# Getting Started

### Requirements

Lelylan is tested against

* Ruby MRI ~1.9.3
* Node ~0.8.8
* MongoDB ~2.6
* Redis ~2.6


## Setup

* [Install MongoDB](https://docs.mongodb.org/manual/installation/)
* [Install Redis](http://redis.io/download)


## Microservices

Lelylan is composed by different microservices. Check out the corresponding repository and follow the installation notes for each of them. 

* [API Proxy](https://github.com/lelylan/api-proxy). Api Proxy.
* [Devices API](https://github.com/lelylan/devices). Monitor and control.
* [Types API](https://github.com/lelylan/types). Device structure (propperties, functions, statuses).
* [Subscriptions API](https://github.com/lelylan/subscriptions). Webhooks subscription.
* [Profiles API](https://github.com/lelylan/profiles). User information.
* [OAuth 2.0](https://github.com/lelylan/people). Authentication and authorization.
* [Physical Proxy](https://github.com/lelylan/physicals). Fire actions to the physical world.
* [MQTT Node](https://github.com/lelylan/nodes). Handle MQTT requests.
* [MQTT Server](https://github.com/lelylan/mqtt). MQTT server/broker 3.1 compliant.
* [Webhooks](https://github.com/lelylan/webhooks). Realtime HTTP notification.
* [Websockets](https://github.com/lelylan/websockets). Full-duplex communication over TCP.

We are studying solutions like Docker, Mesos, and Ansible to simplify the installation process. If you are experimenting in the same area get in touch with [Lelylan Team](http://dev.lelylan.com/api).

## Microservices



# Contributing to Lelylan

https://github.com/docker/docker#how-the-project-is-run
https://github.com/docker/docker/tree/master/project

ROADMAP

### Help

For any problem ask [support](http://dev.lelylan.com/support) to the community and Lelylan Team.


## License

Lelylan is licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).


