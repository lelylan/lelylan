# Lelylan. Open Source Internet of Things


Lelylan is an IoT cloud platform based on a lightweight microservices architecture.

The Lelylan platform is both hardware-agnostic and platform-agnostic. This means that you can connect any hardware, from the ESP8266 to the most professional embedded hardware solution and everything in between - and it can run on any public cloud, your own private datacenter, or even in a hybrid environment, whether virtualized or bare metal.

[![Lelylan Logo](https://raw.githubusercontent.com/lelylan/lelylan/master/public/logo-lelylan.png)](http://lelylan.com)


### Notes 

This repository defines the architecture documentation. Check out the [microservices list](https://github.com/lelylan/lelylan#development) for the code implementation.


### Why Lelylan

Research in the Internet of Things is global and growing fast, but lacks the standard tools. Many companies are building their own solutions. By sharing what we have learned during the years, we want to create a shared code base with a clear focus on developers. To see Lelylan in action checkout the [tutorials](http://dev.lelylan.com/#overview-tutorials) in the dev center. 


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

(remember to run the `mongod` and `redis-server`)

## Setup

* [Install MongoDB](https://docs.mongodb.org/manual/installation/)
* [Install Redis](http://redis.io/download)


## Installation

### Development

Lelylan is composed by different microservices.
Follow the installation guidelines for each of them.

| Microservice  | Description |
| ------------- | ------------- |
| [API Proxy](https://github.com/lelylan/api-proxy) | Proxy API |
| [Devices API](https://github.com/lelylan/devices)  | Device monitoring and control |
| [Types API](https://github.com/lelylan/types) | Device type structure |
| [Subscriptions API](https://github.com/lelylan/subscriptions) | Realtime subscription |
| [Profiles API](https://github.com/lelylan/profiles) | Profile information |
| [OAuth 2.0](https://github.com/lelylan/people) | User authentication and authorization  |
| [Physical Proxy](https://github.com/lelylan/physicals) | Forward requests to the physical world |
| [MQTT Node](https://github.com/lelylan/nodes) | Forward and receive MQTT requests |
| [MQTT Server](https://github.com/lelylan/mqtt) | MQTT server/broker |
| [Webhooks](https://github.com/lelylan/webhooks) | Realtime HTTP notification |
| [Websockets](https://github.com/lelylan/websockets) | Full-duplex communication over TCP |

You can now access the [APIs]((http://dev.lelylan.com/api)) from `http://0.0.0.0:8200` (API proxy URL).


### Production

During deployment, every microservice needs to be set to the following environment variables (remember to change them with your own microservices, mongodb, redis and cache URLs).

| Environment Variable | Description |
| ------------- | ------------- |
| `RACK_ENV=production` | Production rack environment |
| `RAILS_ENV=production` | Production rails environment |
| `NODE_ENV=production` | Production node environment |
| `LELYLAN_PEOPLE_URL=people.lelylan.com` | OAuth 2.0 microservice URL |
| `LELYLAN_DEVICES_URL=devices.lelylan.com` | Devices API microservice URL | 
| `LELYLAN_TYPES_URL=types.lelylan.com` | Types API microservice URL | 
| `LELYLAN_SUBSCRIPTIONS_URL=subscriptions.lelylan.com` | Subs. API microservice URL| 
| `LELYLAN_PROFILES_URL=profiles.lelylan.com` | Profiles API microservice URL | 
| `MONGOLAB_PEOPLE_URL=mongodb://<user>:<pass>@<host>:<port>/<name>` | OAuth 2.0 MongoDB URL| 
| `MONGOLAB_DEVICES_URL=mongodb://<user>:<pass>@<host>:<port>/<name>` | Devices API MongoDB URL| 
| `MONGOLAB_TYPES_URL=mongodb://<user>:<pass>@<host>:<port>/<name>` | Types API MongoDB URL| 
| `MONGOLAB_JOBS_URL=mongodb://<user>:<pass>@<host>:<port>/<name>` | Event Bus MongoDB URL | 
| `MONGOLAB_SUBSCRIPTIONS_URL=mongodb://<user>:<pass>@<host>:<port>/<name>` | Subs. MongoDB URL | 
| `MEMCACHIER_SERVERS=<host>:<port>` | Cache server |
| `MEMCACHIER_USERNAME=<username>` | Cache server username |
| `MEMCACHIER_PASSWORD=<password>` | Cache server password|
| `REDIS_URL` | Background Job Redis URL |
| `REDIS_RATE_LIMIT_URL=redis://<user>:<pass>@<host>:<port>/` | Late Limit Redis URL |

We are studying solutions such as Docker, Mesos, and Ansible to simplify the installation process. If you are experimenting in the same area get in touch with [lelylan team](http://dev.lelylan.com/api).


## Roadmap

The Roadmap provides the description of the items that the project has decided to concentrate on. It should
serve as a reference point for Lelylan contributors to understand where the project is going, and
helps to determine whether a contribution could be conflicting considering the future goals.

The fact that a feature isn't listed here doesn't mean that a patch for it will automatically be
refused (we also miss important things). We are always happy to receive patches for new cool features that we haven't 
thought about, or didn't consider as a priority. Nevertheless understand that such patches might take longer for us 
to review.

Checkout the [roadmap](/ROADMAP.md) to see our near future goals.


## Contributing to Lelylan

This Contributing document tries to define a contributor's guide explaining how to contribute to one or more Lelylan Microservice. It contains information about reporting issues as well as some useful tips and guidelines for experienced open source contributors.

Checkout the [contributing](/CONTRIBUTING.md) to help us with Lelylan.


## Support

Use the available [communication channels](http://dev.lelylan.com/support) to communicate your ideas, problems or suggestions.


## License

Lelylan is licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).


