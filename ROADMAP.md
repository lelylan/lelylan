# Lelylan Roadmap

### How should I use this document?

This document provides description of items that the project decided to prioritize. This should
serve as a reference point for Lelylan contributors to understand where the project is going, and
help determine if a contribution could be conflicting with some longer terms plans.

The fact that a feature isn't listed here doesn't mean that a patch for it will automatically be
refused (we also miss important things). We are always happy to receive patches for new cool features we haven't 
thought about, or didn't judge priority. Please however understand that such patches might take longer for us 
to review.


### How can I help?

Lelylan main objectives are described in [Issues](https://github.com/lelylan/lelylan/issues). Our
goal is to split down the workload in such way that anybody can jump in and help. Please comment on
issues if you want to take it to avoid duplicating effort! Similarly, if a maintainer is already
assigned on an issue you'd like to participate in, pinging him on GitHub to offer your help is
the best way to go.


### Refactoring

Security is a top objective for the Lelylan in the near future. Many microservices have been created
without being upgraded to the latest lib versions which might contain security issues.

- [Framework update](https://github.com/lelylan/lelylan/issues/130)
- Techs update (use the latests stable version of Ruby, Node.js, MongoDB and Redis)

### Test suite refactoring

Lelylan follows best practices on coding style and testing. Many microservices have been created
without having a refactoring for several months and a major refactoring may be needed.

- [Test suite refactoring](https://github.com/lelylan/lelylan/issues/131)

### SDK

Lelylan offers wrappers in different languages like AngularJS, Ruby, Node.js.
We need more SDK in different languages to let more people access the iot.

- [Addition SDK](https://github.com/lelylan/lelylan/issues/126)

### MQTT load tests

In most IOT projects MQTT is a critical block. It doesn't scale easily and consume many resources. Would be nice to make 
different load tests (changing packet size and message ratio) to clearly understand what the MQTT microservice can handle.

### Generic load tests

In most IOT projects MQTT is a critical block. It doesn't scale easily and consume many resources. Would be nice to make 
different load tests (changing packet size and message ratio) to clearly understand what the MQTT microservice can handle.

### Continuous Delivery (DevOps)

The ability to deploy the whole platform with a unique command (or a simplified set of commands) 
using technologies like Docker, Mesos and Ansible would reduce the continuous delivery process.

- [DevOps](https://github.com/lelylan/lelylan/issues/129)

### Documentation

To let engineers, developers and makers use Lelylan is important to create high quality documentation.
We started this through the dev center and the lab, but many things can be done (e.g. video, collaborations 
with online teaching platforms).

- [Documentation](https://github.com/lelylan/lelylan/issues/124)

### Deployment documentation

Lelylan can be deployed in a public cloud or in your own private datacenter, even a hybrid environment. 
It's important to add more documentation showing how to deploy Leylan in a cloud or private datacenter (e.g. using Mesos).

### Better API implementation

The current API miss any versioning support and should be simplified (mainly discussing about the real need of the
Types API). Tools like [apiary.io](https://apiary.io) may also be used to simplify the synch of current APIs with the
documentation.

### Device management

Define a proper device management API (and dashboard). This part requires a full study and before defining its functionalities 
we need to make a deep competitor's analysis.

- [Device Management](https://github.com/lelylan/lelylan/issues/96)

