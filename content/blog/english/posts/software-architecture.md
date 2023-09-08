---
title: "Software Architecture"
date: 2023-08-01
draft: false
description: "Fundamentally, software architecture acts as a blueprint for the organization, operation, and communication of software parts. This ensures the robustness, scalability, and upgradability of the system."
tags: ['architecture', 'softwareengineering']
blog_list_image: images/software-architecture/architecture.jpg
transform: -25%
images: ['images/software-architecture/architecture.jpg']
author: Saúl Zalimben
slug: software-architecture
idiom: English
---


>Architecture is about the important stuff… whatever that is.
>--Ralph Johnson

In this rapidly evolving digital landscape, where innovation and efficiency reign supreme, the role of software architecture has become more critical than ever. Fundamentally, software architecture acts as a blueprint for the organization, operation, and communication of software parts. This ensures the robustness, scalability, and upgradability of the system.

A capable software architect creates a solid and elegant software solution that tackles complicated problems and meets user needs, much as a talented architect creates an impressive skyscraper. The complex balancing act required by software architecture ranges from choosing the right design patterns and technologies to enhancing performance and security while staying within budget and time restrictions.

## Definition
Despite the lack of a clear definition, we can nevertheless benefit from the following definitions of software architecture:

>"In most successful software projects, the expert developers working on that project have a shared understanding of the system design. This shared understanding is called **architecture**."
-- Ralph Johnson

>"Software architecture involves understanding and organising a system, all of its components, their interactions, the environment in which they operate, and the core principles which will be used to design the software."
-- Anna Mleczko

>"Software architecture is the set of structures needed to reason about a software system and the discipline of creating such structures and systems. Each structure comprises software elements, relations among them, and properties of both elements and relations."
-- Wikipedia

So, we will agree on the following definition: 
> Software architecture describes how an application is built including its components, how they interact with each other, the environment in which they operate, and so on. 

![Dimensions of Arquitecture](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ue9jcth1d1lvm798lpq8.png)
Figure 1. *Architecture consists of the structure combined with architecture characteristics (“-ilities”), architecture decisions, and design principles.*

## Dimensions
Software architecture consists of the structure of the system (denoted as the heavy black lines supporting the architecture), combined with architecture characteristics (“-ilities”) the system must support, architecture decisions, and finally design principles. We can refer to these components as **dimensions** of Software Architecture. 

The **structure** of the system refers to the type of architecture style (or styles) the system is implemented in (such as microservices, layered, microkernel, and so on). Describing an architecture only by its structure does not wholly explain the architecture.

For example, if an architect is asked to describe an architecture and that architect responds “It’s a microservices architecture”. Here, the architect is only talking about the structure of the system but not the architecture of the system. 

*Knowledge of the architecture characteristics, architecture decisions, and design principles are also needed to fully understand the architecture of the system.*

![Structure dimension](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/i3l0oqapmmmjb8x2zv6i.png)
Figure 2. *Structure refers to the type of architecture styles used in the system.*

**Architecture characteristics** are another dimension of defining software architecture. The architecture characteristics define the success criteria of a system, which is generally orthogonal to the functionality of the system. 

In general, the characteristics do not need knowledge of the functionality of the system, yet they are required in order for the system to function properly.

![Architecture characteristics dimension](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1yoj13crfdi0b9vrshka.png)
Figure 3. *Architecture characteristics refers to the “-ilities” that the system must support*

**Architecture decisions** define the “rules” for how a system should be constructed. For example, an architect might make an architecture decision that only the business and services layer within a layered architecture may access the database, thus restricting the presentation layer from making direct database calls. 

Architecture decisions form the constraints of the system and direct the development teams on what is and what isn’t allowed.

![Architecture decisions dimension](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/epnp245ev6zn7akwht60.png)
Figure 4. *Architecture decisions are rules for constructing systems.*

**Design Principles** differ from an architecture decision in that a design principle is a guideline rather than a hard-and-fast rule. 

For example, a design principle can state that the development teams should leverage asynchronous messaging between services within a microservices architecture to increase performance. 

An architecture decision (rule) could never cover every condition and option for communication between services in an architecture decision, so a design principle can be used to provide guidance for the preferred method (in this case asynchronous messaging) to allow the developer to choose a more appropriate communication protocol (such as REST or gRPC) given a specific circumstance.

![Design principles dimension](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/5fsc538tumd6eilwjj0e.png)
Figure 5. *Design principles are guidelines for constructing systems.*

## Laws of Software Architecture
Although the range of software design is wide, there are unifying characteristics. The first law was discovered by Mark Richards and Neal Ford by accident as they kept running against it: 
> **Everything in software architecture is a tradeoff.**
—1st Law of Software Architecture

Nothing exists on a nice clean spectrum for software architects—every decision must take into account many opposing factors.

> **If an architect thinks they have discovered something that isn’t a tradeoff, more likely they just haven’t identified the tradeoff yet.**
—Corollary 1

## Resources
- Richards, M. (2022). Software architecture patterns. 2nd Edition.
- Richards, M., & Ford, N. (2020). Fundamentals of software architecture: an engineering approach. O'Reilly Media.
- Ozkaya, M. Design Microservices Architecture with Patterns & Principles [MOOC]. Udemy. https://www.udemy.com/course/design-microservices-architecture-with-patterns-principles/
- Fowler, M. (2019, August 1). Software Architecture Guide. Martin Fowler. https://martinfowler.com/architecture/

## Acknowledgements
- Cover image by [Alex wong](https://unsplash.com/@killerfvith) on [Unsplash](https://unsplash.com/license)
- Content images were extracted from Richards, M. (2022) and Richards, M., & Ford, N. (2020).