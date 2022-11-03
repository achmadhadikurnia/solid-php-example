# What is SOLID Principles?
SOLID is an acronym for the first five object-oriented design (OOD) principles and is a series of guidelines that developers can use to build software in an easy way to maintain and extend. Understanding these concepts will make you a better developer and enable you to avoid code smells.

## Why should I use them?
- Software design principles or conventions.
- Widely accepted in the industry.
- Help make code more maintainable and tolerant to changes.
- Applicable in terms of class design (micro-design), and also at the software architecture level.

### If you don't use SOLID, you probably code STUPID¹ without knowing it
STUPID stands for Singleton, Tight Coupling, Untestability, Premature Optimization, Indescriptive Naming, Duplication

## What does SOLID stands for
SOLID is an acronym that stands for:
- Single responsibility principle
- Open/closed principle
- Liskov substitution principle
- Interface segregation principle
- Dependency inversion principle

## Let’s dive in deeper those principles!
### S - Single Responsibility Principle (SRP) ([Example](./1-single-responsibility-principle.md))
This principle is about **actors and high level architecture**.
> A class should have one, and only one, reason to change.

### O - Open-Closed Principle (OCP) ([Example](./2-open-closed-principle.md))
This principle is about **class design and feature extensions**.
> A class should be open for extension, but closed for modification.

### L - Liskov Substitution Principle (LSP) ([Example](./3-liskov-substitution-principle.md))
This principle is about **subtyping and inheritance**
> Derived classes must be substitutable for their base classes.

### I - Interface Segregation Principle (ISP) ([Example](./4-interface-segregation-principle.md))
This principle is about **business logic to clients communication**.
> Many client-specific interfaces are better than one general-purpose interface.

### D - Dependency Inversion Principle (DIP) ([Example](./5-dependency-inversion-principle.md))
This principle wires up all **other four principles in a single circle**.
> Depend upon abstractions. Do not depend upon concretions.

## Conclusion
SOLID isn't a perfect methodology, and can lead to complex applications with many moving parts, and occasionally lead to writing code just in case it's needed. Using SOLID means writing more classes and creating more interfaces, but many modern IDE's will solve that problem through automated code completion.

That said, it does force you to separate concerns, to think about inheritance,
prevent repeating code and carefully approach writing applications. Thinking
about how objects fit together in an application is, after all, what object
oriented code is all about.
