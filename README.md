# Clean Architecture

## Chapter 1: Design & Architecture
### Goal
The goal of software architecture is to minimise the human resources required to build & maintain the required system.

### Metrics
- Lines of code over time
- Cost per line of code
- Productivity over time

## Chapter 2: A Tale of Two Values
### Behaviour vs Architecture

Consider importance & urgency matrix. In most cases, business logic (behaviour) is considered more urgent and architecture may never be urgent in the eyes or business managers.

Consider the extreme, new features can be easily added to a system with very good architecture. System with too many features, but poor architecture may end up becoming impossible for additional features to be added in.

## Chapter 3 - 6: Programming Paradigms

- Structured Programming: impose discipline on direct transfer of control
  - ability to create falsifiable units of programming
  - functional decomposition recursively breaks down a big problem to many small ones
  - Dijkstra, "tests show the presence, not the absence, of bugs". Software is like a science, which shows correctness by failing to prove incorrectness.
- OOP: impose discipline on indirect transfer of control
  - OO: combination of data & function
  - a way to model the real world
  - encapsulation (to expose only a subset of functions & data); inheritance (more conveniently play with data structure and reuse code); polymorphism: allows dependency inversion, which allows engineers to have absolute control over every source code dependency in the system
- Functional Programming: impose discipline upon assignment
  - **immutability:** no concurrency issue
  - **event sourcing:** store only the transactions, not the state. Instead of CRUD, just CR. Assuming unlimited storage and processing power, the system is entirely functional. (how source control system works)

Essentially: software is composed of sequence, selection, iteration, and indirection. Nothing more, nothing less.

## Chapter 7 - 11: Design Principles
#### Goal of the principle is to create mid-level software structures that:
- tolerate change
- easy to understand
- basis of components that can be used in many software systems

The famous SOLID Principles:
![pic](./solid.jpg)
