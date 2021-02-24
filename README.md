# Awesome Event-driven Architecture

A collection for event-driven architecture

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [Awesome Event-driven Architecture](#awesome-event-driven-architecture)
  - [Definition](#definition)
    - [Gartner](#gartner)
    - [IBM](#ibm)
    - [Wiki](#wikihttpsenwikipediaorgwikievent-driven_architecture)
  - [Tutorial](#tutorial)
  - [Video](#video)
  - [Book](#book)

<!-- /code_chunk_output -->

## Definition

### Gartner

> **Event-driven architecture (EDA)** is a design paradigm in which a software component executes in response to receiving one or more event notifications. EDA is more loosely coupled than the client/server paradigm because the component that sends the notification doesn’t know the identity of the receiving components at the time of compiling.


### IBM
 
> Event-driven architecture is an integration model built around the publication, capture, processing, and storage (or persistence) of events. Specifically, when an application or service performs an action or undergoes a change that another application or service might want to know about, it publishes an event—a record of that action or change—that another application or service can consume and process to perform one or more actions in turn.
>
> Event-driven architecture enables a *loose coupling* between connected applications and services—they can communicate with each other by publishing and consuming events without knowing anything about each other except the event format. This model offers significant advantages over a *request/response* architecture (or integration model), in which one application or service must request specific information from another specific application or service that is expecting the specific request.

### [Wiki](https://en.wikipedia.org/wiki/Event-driven_architecture)

> Event-driven architecture (EDA) is a software architecture paradigm promoting the production, detection, consumption of, and reaction to events.

## Tutorial

- [What Is Event Driven Architecture, and When Should I Use It?](https://medium.com/swlh/what-is-event-driven-architecture-and-when-should-i-use-it-cb30ae68899a)

> Event-driven architecture is a software architecture paradigm promoting the production, detection, consumption of, and reaction to events.

> There are a few reasons why using an event driven architecture can be an advantage over alternative architectures.
> 
> **Loose coupling** — Services do not need to be dependent on each other. This applies different factors such as transport protocol, availability (the service being online) and the data being sent. The consumer will still need to know how to interpret an event or message so a strict contract should still be used between the two services, but implementation details of the contract should not matter.
> 
> **Scalability** — Since the services are no longer coupled, the throughput of service 1, no longer needs to meet the throughput of service 2. This can help reduce costs as services no longer need to be online 24/7 and it is possible to take advantage of serverless computing with infinite scaling.
> 
> **Asynchronicity** — Since services are no longer dependent on a result being returned synchronously, a fire and forget model can be used, which can greatly speed up a process. This can have a downside, which will be outlined below.
> 
> **Point in time recovery** — If events are backed by a queue or maintaining some kind of history, it is possible to replay events, or even go back in time and recover state.
> 
> There are drawbacks to using an event driven architecture as well.
> 
> **Over-engineering of processes** — Sometimes a simple call from one service to another is enough. If a process uses event driven architecture, it usually requires much more infrastructure to support it, which will add costs (as it will need a queueing system)
> 
> **Inconsistencies** — Because processes now rely on eventual consistency, it is not typical to support ACID (atomicity, consistency, isolation, durability) transactions, so handling of duplications, or out of sequence events can make service code more complicated, and harder to test and debug all situations.

- [Introduction to Event-Driven Architecture](https://medium.com/microservicegeeks/introduction-to-event-driven-architecture-e94ef442d824)

> **Event-driven Architecture (EDA)** is a software architecture paradigm promoting the production and consumption of **events**.

> A producer ensures that everything that a prospective consumer needs to process the event is captured. 

![Event-Driven Architecture Reference Model
](assets/1.png)

![Benefits and drawbacks of event-driven architecture
](assets/2.png)

- [Make legacy applications first-class citizens of event-driven architectures via cloud, DevOps and CDC](https://www.thoughtworks.com/insights/blog/make-legacy-applications-first-class-citizens-event-driven-architectures-cloud-devops-and)

- [Gartner on Event-Driven Architecture: A Foundational Element of Digital Business](https://solace.com/blog/gartner-on-event-driven-architecture/)

- [AWS - What is an Event-Driven Architecture?](https://aws.amazon.com/event-driven-architecture/)
![How it works: example architecture
](./assets/3.png)

## Video

- [Martin Fowler - The Many Meanings of Event-Driven Architecture](https://youtu.be/STKCRSUsyP0)
- [Event-Driven Architecture – Benefits and Pitfalls](https://youtu.be/ZuXqW8aKxc4)

## Book

- [O’Reilly - Building Event-Driven Microservices](https://www.oreilly.com/library/view/building-event-driven-microservices/9781492057888/)

- [Microsoft - Exploring CQRS and Event Sourcing](https://www.microsoft.com/en-sg/download/details.aspx?id=34774)
