# Lelylan. Open Source Internet of Things

Lelylan is an iot cloud platform based on a lightweight microservices architecture.

Lelylan platform is both hardware-agnostic and platform-agnostic. This means you can connect any hardware, from the ESP8622 to the most professional embedded hardware solution and everything in between - and it can run on any public cloud or in your own private datacenter, or even a hybrid environment, whether virtualized or on bare metal.

![Lelylan Logo](https://raw.githubusercontent.com/lelylan/lelylan/master/public/logo-lelylan.png)

### Why Lelylan

Research in the Internet of Things is global and growing fast, but lacks standard tools. Many companies are building their own solution. By sharing what we have learned during the years, we want to create a shared code base for the Internet of Things. To see Lelylan in action checkout the [tuturials](http://dev.lelylan.com/#overview-tutorials) in the dev center. 

### Resources

* [Architecture](http://dev.lelylan.com/architecture) (request life cycle)
* [Internet of Things API](http://dev.lelylan.com/api) (how it works)
* [Blog](http://lelylan.com) (latest from the community)



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

Lelylan is composed by different microservices. Follow the installation process for each of them. 

* [Devices API](https://github.com/lelylan/devices) (device monitor and control)
* [Types API](https://github.com/lelylan/types) (device structure definition)
* [Subscriptions API](https://github.com/lelylan/subscriptions) (realtime webhooks subscription)
* [Profiles API](https://github.com/lelylan/profiles) (user information)
* [OAuth 2.0](https://github.com/lelylan/people) (authentication and authorization)
* [Physical Proxy](https://github.com/lelylan/physicals) (forward actions to the physical world)
* [MQTT Node](https://github.com/lelylan/nodes) (handle MQTT requests)
* [MQTT Server](https://github.com/lelylan/mqtt) (MQTT server/broker 3.1 compliant)
* [Webhooks](https://github.com/lelylan/webhooks) (realtime HTTP notification)
* [Websockets](https://github.com/lelylan/websockets) (full-duplex communication over TCP)
* [API Proxy](https://github.com/lelylan/api-proxy) (API access point)

We are studying solutions like Docker, Mesos, and Ansible to simplify the installation process. If you are experimenting in the same area get in touch with [lelylan team](http://dev.lelylan.com/api).


## Contributing

Fork the microservice repo on github and send a pull requests with topic branches. Do not forget to
provide specs to your contribution.


# Contributing to Lelylan

https://github.com/docker/docker#how-the-project-is-run
https://github.com/docker/docker/tree/master/project

ROADMAP

### Help

For any problem ask [support](http://dev.lelylan.com/support) to the community and Lelylan Team.


## License

Lelylan is licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).


