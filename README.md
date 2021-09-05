# Research: Domain Driven Design

### Description

## Domain Driven Design – 10 study points
Research the Internet and/or the recommended books and find the answers of the following questions:

#### ● what is DDD?
"
DDD is a software development approach that uses and builds upon OOAD () principles and ideas.
Domain in the realm of software engineering commonly refers to the subject area on which the application is intended to apply. In other words, during application development, the domain is the “sphere of knowledge and activity around which the application logic revolves.”
"
[AirBrake - Blog Source on DDD](https://airbrake.io/blog/software-design/domain-driven-design)
Personal note: DDD seems to be concerned with translating the real world business logic into application logic.

"

DDD focuses on three core principles:

    Focus on the core domain and domain logic.
    Base complex designs on models of the domain.
    Constantly collaborate with domain experts, in order to improve the application model and resolve any emerging domain-related issues.

Evans’ Domain-Driven Design further defines a few common terms that are useful when describing and discussing DDD practices:

    Context:
    The setting in which a word or statement appears that determines its meaning. Statements about a model can only be understood in a context.
    Model:
    A system of abstractions that describes selected aspects of a domain and can be used to solve problems related to that domain.
    Ubiquitous Language:
    A language structured around the domain model and used by all team members to connect all the activities of the team with the software.
    Bounded Context:
    A description of a boundary (typically a subsystem, or the work of a specific team) within which a particular model is defined and applicable.
"

[AirBrake - Blog Source on DDD](https://airbrake.io/blog/software-design/domain-driven-design)

#### ● when did it originate?
"Initially introduced and made popular by programmer Eric Evans in his 2004 book, Domain-Driven Design: Tackling Complexity in the Heart of Software"
[AirBrake - Blog Source on DDD](https://airbrake.io/blog/software-design/domain-driven-design)
#### ● which problems did it address?

- Eases Communication: 
Simple and agreed upon terms will make it easier to communicate about non-simple terms and logic.
- Improves Flexibility:
DDD is flexible because of the advantages that being based upon Object-Oriented analysis and Design. 
- Emphasizes Domain Over Interface:
With the focus being on the domain (the actual business logic and subject area) rather than the interface, it will also translate to usefulness in aggregating value     for the business as long as the UI/UX doesn't directly detract from that.

#### ● which are the basic concepts and building blocks of a domain model

"
- Entity: 
    An object that is identified by its consistent thread of continuity, as opposed to traditional objects, which are defined by their attributes.
    Value Object:
    An immutable (unchangeable) object that has attributes, but no distinct identity.
- Domain Event: 
    An object that is used to record a discrete event related to model activity within the system. While all events within the system could be tracked, a domain event is     only created for event types which the domain experts care about.
- Aggregate: 
    A cluster of entities and value objects with defined boundaries around the group. Rather than allowing every single entity or value object to perform all actions on     its own, the collective aggregate of items is assigned a singular aggregate root item. Now, external objects no longer have direct access to every individual entity     or value object within the aggregate, but instead only have access to the single aggregate root item, and use that to pass along instructions to the group as a           whole. This practice correlates with many of the actual coding practices we’re covering in our design patterns series.
- Service:
    Essentially, a service is an operation or form of business logic that doesn’t naturally fit within the realm of objects. In other words, if some functionality must 
    exist, but it cannot be related to an entity or value object, it’s probably a service.
- Repositories:
    Not be confused with common version control repositories, the DDD meaning of a repository is a service that uses a global interface to provide access to all entities 
    and value objects that are within a particular aggregate collection. Methods should be defined to allow for creation, modification, and deletion of objects within 
    the aggregate. However, by using this repository service to make data queries, the goal is to remove such data query capabilities from within the business logic of 
    object models.
- Factories:
    As we’ve discussed through a number of design patterns articles already, DDD suggests the use of a factory, which encapsulates the logic of creating complex objects 
    and aggregates, ensuring that the client has no knowledge of the inner-workings of object manipulation.

"
[AirBrake - Blog Source on DDD](https://airbrake.io/blog/software-design/domain-driven-design)

#### ● how does DDD relate to microservices architecture?

This is an individual task.

## Authors
Frederik Blem.
