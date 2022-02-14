---
title: Training 06 - Architecture (Software)
date: 2020-10-09
authors: Hing-Wah.Kwok@dst.defence.gov.au, Philip.Cutler@dst.defence.gov.au
---

<!-- # Training 06 - Architecture (Software) -->
## Microservice architecture overview

> *The microservice architectural style is an approach to developing a single application as a suite of small services, each running in its own process and communicating with lightweight mechanisms* - James Lewis and Martin Fowler, Thoughtworks

A microservice architecture is a development practice where you separate parts of an application into sections, each called a microservice. Each microservice:
* is a small distinct section of the application
* does something specific
* is often packaged into an individual container
* communicates with other microservices
* can be independently deployed.

To use a microservice architecture, you should embrace agile and DevOps practices.

### Benefits of a microservice architecture

* Faster customer feedback, get parts of the product in front of customer faster
* Quicker and simpler to identify and fix issues
* Reduced security issues with each section being separated from the rest
* Changes are simplified since you can modify and deploy only the microservice and not the whole application
* Not limited to any specific programming languages or system
* Easy to scale

### Implementing a microservice architecture

Designing a microservice architecture takes careful thought and consideration. It is an iterative process, and the design can change over time. Following a domain-driven design (DDD) framework can help.

For a brief example demonstrating a domain analysis with DDD, and identifying microservices, see [Using domain analysis to model microservices](https://docs.microsoft.com/en-us/azure/architecture/microservices/model/domain-analysis#:~:text=A%20bounded%20context%20is%20simply,necessarily%20isolated%20from%20one%20another.) by Microsoft.

#### Migrating a monolithic application to microservices

It's possible to transition a monolith to a microservices architecture by following a process called "Killing the monolith". The idea behind this process is to slowly take parts of the monolithic application and replace them with microservices over time, until eventually the entire monolith is no longer in use.

To read about how one organisation implemented this practice, see [Killing a Monolith — How Smartly.io Reworked their Architecture](https://www.smartly.io/blog/killing-a-monolith-how-smartly.io-reworked-their-architecture) by Oskari Virtanen.

#### Size of a microservice

There is no ideal size for a microservice. Each microservice should do one thing.

Microservices should be:
*   designed around business capabilities, not horizontal layers like data access or messaging
*  loosely coupled, to be able to update one microservice without having to update any others
* cohesive, by having a single, defined purpose.

#### Dedicated teams

* Each microservice can have a dedicated team.
* Adopting DevOps or agile processes helps enable open communication between teams.
* Each team can have a different database.
    * This will need data synchronisation to keep data replication up to date across different databases.
* Each team can use different code repositories.
* There is usually a user interface team.

#### Microservice communication

There are two main communication types used to have microservices communicate with each other:
* Remote procedure invocation, which has one microservice message the other microservice directly, and receive a response. For example, REST/SOAP.
* Lightweight messaging, which uses a broker to manage the messages. Each service messages the broker, and is subscribed to the broker. For example, Apachi Kafka, RabbitMQ.

#### Service registry

A service registry can be used to track the location of microservice instances, since network locations can change dynamically. For this, microservices register their network location on start up, and deregister on shutdown.

Service registry tool examples include Eureka, Zookeeper, Consul.

## Introductory References

### Articles

- Microservice Architectures
  - [Microservices: a definition of this new architectural term](https://martinfowler.com/articles/microservices.html)
- Cloud Native Architecture
  - [Cloud Native Applications](https://tanzu.vmware.com/cloud-native)
  - [Cloud Native Application Architecture](https://medium.com/walmartglobaltech/cloud-native-application-architecture-a84ddf378f82)
  - [CNCF Cloud Native Definition](https://github.com/cncf/toc/blob/master/DEFINITION.md)

### Books

- [Building Microservices, 2nd Edition Book](https://learning.oreilly.com/library/view/building-microservices-2nd/9781492034018/) - by Sam Newman
- [Building Evolutionary Architectures Book](https://learning.oreilly.com/library/view/building-evolutionary-architectures/9781491986356/) - by Neal Ford, Rebecca Parsons and Patrick Kua
- [Cloud Native Book](https://learning.oreilly.com/library/view/cloud-native/9781492053811/)
- [Domain-Driven Design: Tackling Complexity in the Heart of Software Book](https://learning.oreilly.com/library/view/domain-driven-design-tackling/0321125215/)

### Video Playlists

- [Sam Newman: Monolith to Microservices](https://www.infoq.com/podcasts/monolith-microservices/)

## Technologies
