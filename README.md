# Lelylan: Open Source Internet of Things

Lelylan is an iot cloud platform based on a lightweight microservices architecture.

Lelylan platform is both hardware-agnostic and platform-agnostic. This means you can connect any hardware, from the ESP8622 to the most professional embedded hardware solution and everything in between - and it can run on any public cloud or in your own private datacenter, or even a hybrid environment, whether virtualized or on bare metal.

![Lelylan Logo](https://raw.githubusercontent.com/lelylan/lelylan/master/public/logo-lelylan.png)

## Why Lelylan

Research in the Internet of Things is global and growing fast, but lacks standard tools. Many companies are building their own solution. By sharing what we have learned during the last years, we hope to create a shared iot platform for connected products.

## Usage Examples

To see Lelylan in action checkout the [tuturials](http://dev.lelylan.com/#overview-tutorials) in the dev center.

## Beta Limitations

We do our best to provide a highly secure, reliable, scalable, and resilient service. However, Lelylan is still in beta and problems may occour. Use the [support channels](http://dev.lelylan.com/support) to get in touch with the Lelylan team and the community.



# Getting Started

Lelylan can be installed either on your computer or on servers. Before installing Lelylan you may find useful to read more about the [architecture](http://dev.lelylan.com/architecture) and the [APIs](http://dev.lelylan.com/api).

## Requirements

Lelylan API is tested against MRI 1.9.3.
Devices API is tested against MRI 1.9.3.

## Lelylan Microservices

Lelylan is composed by a number of microservices (small apps) under development and each of them has its own installation instructions. 

Docker Registry: Registry server for Docker (hosting/delivery of repositories and images)
Docker Machine: Machine management for a container-centric world
Docker Swarm: A Docker-native clustering system
Docker Compose (formerly Fig): Define and run multi-container apps
Kitematic: The easiest way to use Docker on Mac and Windows
If you know of another project underway that should be listed here, please help us keep this list up-to-date by submitting a PR.

## Under the hood

Under the hood, Lelylan is built using the following components:

* The Ruby and Node.js programming languages.
* The MongoDB document-oriented database.
* The Redis in-memory data structure store.

# Contributing to Lelylan

https://github.com/docker/docker#how-the-project-is-run
https://github.com/docker/docker/tree/master/project


## License

Lelylan is licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).


