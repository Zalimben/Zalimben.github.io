---
title: "Software Architecture Styles"
date: 2023-10-23
draft: false
description: "Architecture styles help define the basic characteristics and behavior of an application."
tags: ['architecture', 'softwareengineering']
blog_list_image: images/software-architecture/architecture-styles.jpg
transform: -25%
images: ['images/software-architecture/architecture-styles.jpg']
author: Saúl Zalimben
slug: software-architecture-styles
idiom: English
---

Architecture styles help define the basic characteristics and behavior of an application. Some styles lend themselves to highly scalable systems, whereas others lend themselves to applications that allow developers to respond quickly to change.

Knowing each architecture style’s characteristics, strengths, and weaknesses is necessary to choose the one that meets your specific business needs and goals.

- **Architecture styles** describe the macrostructure of a system. An architectural style improves partitioning and promotes design reuse by frequently solving recurring problems.

- **Architecture patterns**, on the other hand, describe reusable structural building block patterns that can be used within each of the architectural styles to solve a particular problem.
They provide a structured solution to architectural issues, detailing how components and interactions should be structured for specific functionality.

![Architecture styles vs architecture patterns](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/vq4m87e0ow9jw702q665.png)
*Architecture styles can be composed of architectural patterns, which in turn can be composed of design patterns.*

An architecture style can be composed of architectural patterns, which in turn can be composed of design patterns. Design patterns and architecture patterns are typically combined to form a complete solution.

Architecture styles act in the same way, they can also be combined when building software solutions to form a complete solution.
Hybrid architectural styles are common in the real world because not every architectural style can solve every business problem.

The separation of what is architectural and what is design is not commonly agreed upon, nor are the patterns cataloged in any accepted form.

## Architecture Classification
Architecture styles are classified as belonging to one of two main architectural structures: **monolithic** (single deployment unit) and **distributed** (many deployment units, usually consisting of services).

![Monolithic Architectures](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ix8z8qjia93nq85omy4h.png)
*Monolithic architectures are single deployment units.*

While cost and simplicity are the main strong points of a monolithic architecture, operational characteristics such as scalability, fault tolerance, and elasticity are its weak points.

Moreover, mean time to recovery (MTTR) and mean time to start (MTTS) are usually measured in minutes, meaning that once a failure does occur, it takes a long time for the application to start back up. These long startup times also impact scalability and elasticity.

#### What is Monolithic Architecture?
- Monolithic architecture is an architectural style of designing and developing complete applications as a **single unit**. For example, a traditional application will have a frontend API service, a load balancer, and a database.
- In this style, everything from user interface, business codes, and data access operations is included in the same code base. If all the functionalities of a project exist in a single code base, then that application is known as a monolithic application.

#### Advantages and disadvantages

Since the project is a single code base, it is easy to pull and get started to develop. It is easy to debug business interactions across different modules.

It becomes too large in code size with time. That's why it's difficult to manage, to work in parallel in the same code base, and to implement new features. Any changes need deploying the entire application and so on.

#### When to Consider This Style

If you are building a small app, go with monolithic architecture because it's simpler. Building, testing, deploying, and troubleshooting them is simple. Scaling up is quick and easy. It is easier to deploy as only a single jar or war file is deployed.

Also, this style should be considered if your team is small, around 3 to 5 people. You can meet all your business needs without dealing with extra architectural complexity. Focus on the business side, not the latest technology options.

You can also use this when making a basic app with a known size and difficulty level. If your application is not very complex and doesn't need to handle a large amount of data, a monolithic architecture is a good choice.

This architecture is a good fit to build a proof of concept and quick launch. This way, you can test your idea and decide to pivot or wrap up the project very fast. 

### Headless Architectures

Headless architecture separates the website's frontend (UI) and backend (business logic). This way, businesses gain maneuverability and flexibility. This is a step towards distributed architectures like microservices.

![Headless Architecture](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/0ddbov97fmk9kyrxgram.png) *Headless architectures consist of decoupling the frontend (presentation layer) and the backend (business logic) layers of a system*.

It uses APIs to connect the frontend and backend applications, while the frontend and backend aren't tightly coupled in headless architectures, they need to communicate with each other using the APIs.

#### Advantages and disadvantages

This architecture separates the frontend and backend layers of a system so developers can make changes to either the frontend or backend without affecting the other component.

The frontend can be deployed independently of the backend (and vice versa). But, if they are not in sync or the compatibility is broken the whole system would fail.

The presentation layer is detached, but it still has the same drawbacks as monolithic architectures.

### Modular Monolithic Architectures
A modular monolith architecture is a software development approach that uses one big codebase, like monolithic architecture. However, the codebase is divided into separate modules. Each module can be developed, tested, and maintained independently.

Each module is designed to be loosely coupled, meaning that changes to one module won’t affect any other. This allows a team to work on their own parts of the codebase without understanding the whole system. This makes it much faster and easier to make changes or add new features.

![Modular Monolithic Architectures](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/3893k8lgmlqf2pe42spn.png)
*Modular monolithic architectures divide the codebase logically into many modules.*

#### Advantages and disadvantages
With this approach, productivity is increased by using a single codebase. Because developers are able to spot and fix problems as they arise. Developing a module doesn't need any infrastructure or continuous integration, no databases are required either. Modules can be added quickly.

A simpler architecture than microservices, without needing extra tools like API Specifications or Message Brokers, Service Discovery, and so on. Yet, the project can be easily transformed into a microservice architecture by splitting the program into different services.

Unfortunately, the codebase is divided into modules but not as deployment units. This means it has the same drawbacks as monolithic architectures.

### Distributed Architectures

Distributed architectures consist of multiple deployment units that work together to perform some sort of cohesive business function.

![Distributed Architectures](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rxlziqvgfnfq7zaqfx10.png)
*Distributed architectures consist of multiple deployment units*.

The superpowers of distributed architectures usually fall within operational characteristics—things like scalability, elasticity, fault tolerance, and in some cases, performance. 

Scalability and elasticity are usually at the service level in these architectural styles. Therefore, the time it takes to start and recover from errors in a modular application is significantly shorter. This time is usually measured in seconds, and sometimes even in milliseconds, instead of minutes.

#### Advantages and disadvantages

The ability to respond quickly to change is a superpower of distributed architectures. Breaking down the application into smaller units makes it easier to find and make changes. This also reduces the amount of testing needed and lowers the risk of deployment.

However, distributed architectures have a problem called the **fallacies of distributed computing**.

>The fallacies of distributed computing are a set of assertions describing false assumptions that programmers new to distributed applications invariably make. These fallacies  are:
>- The network is reliable
>- Latency is zero
>- Bandwidth is infinite
>- The network is secure
>- Topology doesn't change
>- There is one administrator
>- Transport cost is zero
>- The network is homogeneous

### Which One Should I Choose?
If you're deciding between a monolithic or distributed architecture, ask yourself which characteristics your system needs to support.

When systems have different architectural characteristics, they often need a distributed architecture. One example is when customers need a feature that can handle lots of users, respond quickly, be available all the time, and adapt easily. Also, a backend processing functionality that doesn’t need any of those characteristics.

Simple systems or websites usually work best with a simpler and cheaper architecture style. Complex systems that do many business functions work best with more complex distributed architectures. 

Distributed architectures are good for high speed, scalability, and fault tolerance.

When choosing between a **monolithic** or **distributed architecture**, some important questions to ask yourself are:
- What are the architectural characteristics that must be supported?
- What are the needs that must be covered?

#### Monolith First
Distributed architectures are useful, but their supporters admit that using them comes with a big "Premium" problem. This means they are only useful for more complicated systems, not for all. This premium issue, which is the cost of managing services, will slow down a team, favoring a monolith for simpler applications. 

A strong argument is made for starting with a monolith-first strategy. You should build a new application as a monolith, even if you think it will need a distributed architecture later.

The logical way is to design a monolith carefully, focusing on making the software modular and organizing the data correctly. Pay attention to API boundaries and how the data is stored. If you do this well, it's quite easy to transition to distributed architectures.

A more common approach is to start with a monolith and gradually peel off small services at the edges. Such an approach can leave a substantial monolith at the heart of the microservices architecture, but with most new developments occurring in the microservices the monolith is relatively quiescent.

Another common approach is to just replace the monolith entirely. Don't worry about creating a monolith that you'll eventually get rid of, especially if it helps you launch quickly.

![Architectures styles by deployment](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/s1n2hgzzz5gd5cafq6lf.png)
*Monolith First Strategy*.

>You shouldn't start with microservices unless you have reasonable experience in building a microservices system in the team.

## Resources
1. Richards, M. (2022). Software architecture patterns. 2nd Edition.
2. Richards, M., & Ford, N. (2020). Fundamentals of software architecture: an engineering approach. O'Reilly Media.
3. Ozkaya, M. Design Microservices Architecture with Patterns & Principles [MOOC]. Udemy. https://www.udemy.com/course/design-microservices-architecture-with-patterns-principles/
4. Fowler, M. (2019, August 1). Software Architecture Guide. Martin Fowler. https://martinfowler.com/architecture/
5. Fowler, M. (2015, June 3). MonolithFirst. Martin Fowler. https://martinfowler.com/bliki/MonolithFirst.html

## Acknowledgements
- Cover image by [@Uwe Hensel](https://unsplash.com/@sonnar_mc) on [Unsplash](https://unsplash.com/license)

