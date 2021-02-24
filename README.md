# awesome-eda {ignore=true}

A collection for event-driven architecture

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [awesome-eda {ignore=true}](#awesome-eda-ignoretrue)
- [Tutorial](#tutorial)
- [Video](#video)

<!-- /code_chunk_output -->

# Tutorial

- [What Is Event Driven Architecture, and When Should I Use It?](https://medium.com/swlh/what-is-event-driven-architecture-and-when-should-i-use-it-cb30ae68899a)

> Event-driven architecture is a software architecture paradigm promoting the production, detection, consumption of, and reaction to events.

> There are a few reasons why using an event driven architecture can be an advantage over alternative architectures.
> **Loose coupling** — Services do not need to be dependent on each other. This applies different factors such as transport protocol, availability (the service being online) and the data being sent. The consumer will still need to know how to interpret an event or message so a strict contract should still be used between the two services, but implementation details of the contract should not matter.
> **Scalability** — Since the services are no longer coupled, the throughput of service 1, no longer needs to meet the throughput of service 2. This can help reduce costs as services no longer need to be online 24/7 and it is possible to take advantage of serverless computing with infinite scaling.
> **Asynchronicity** — Since services are no longer dependent on a result being returned synchronously, a fire and forget model can be used, which can greatly speed up a process. This can have a downside, which will be outlined below.
> **Point in time recovery** — If events are backed by a queue or maintaining some kind of history, it is possible to replay events, or even go back in time and recover state.
> There are drawbacks to using an event driven architecture as well.
> **Over-engineering of processes** — Sometimes a simple call from one service to another is enough. If a process uses event driven architecture, it usually requires much more infrastructure to support it, which will add costs (as it will need a queueing system)
> **Inconsistencies** — Because processes now rely on eventual consistency, it is not typical to support ACID (atomicity, consistency, isolation, durability) transactions, so handling of duplications, or out of sequence events can make service code more complicated, and harder to test and debug all situations.

- [Introduction to Event-Driven Architecture](https://medium.com/microservicegeeks/introduction-to-event-driven-architecture-e94ef442d824)

> **Event-driven Architecture (EDA)** is a software architecture paradigm promoting the production and consumption of **events**.

> A producer ensures that everything that a prospective consumer needs to process the event is captured. 

![Event-Driven Architecture Reference Model
](assets/1.png)

![Benefits and drawbacks of event-driven architecture
](assets/2.png)

- [Make legacy applications first-class citizens of event-driven architectures via cloud, DevOps and CDC](https://www.thoughtworks.com/insights/blog/make-legacy-applications-first-class-citizens-event-driven-architectures-cloud-devops-and)


# Video

- [Event-Driven Architecture – Benefits and Pitfalls](https://youtu.be/ZuXqW8aKxc4)