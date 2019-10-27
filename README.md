# Type problems
A set of problems to improve your skills with `TyDD, Type Driven Development` 
in Java and some Functional libraries.

## Motivation

Using Java, the developers implements the solutions, transforming data 
with different nature. We will consider that data as `Values`. That values will be encapsulated into Business Objects. For the design of your 
values, you will use [Java primitives](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)
or [Java wrapper classes](https://en.wikipedia.org/wiki/Primitive_wrapper_class):

![](docs/images/javaTypes.png) 

From Java 8, you can use `Monads`, a parameterized Types to model data with
complex state. What Monads are available in Java 8+?

- [Stream< T >](https://docs.oracle.com/javase/8/docs/api/java/util/stream/Stream.html)
- [Optional< T >](https://docs.oracle.com/javase/8/docs/api/java/util/Optional.html)
- [CompletableFuture< T >](https://docs.oracle.com/javase/8/docs/api/java/util/concurrent/CompletableFuture.html)

Using third party libraries like VAVR, you could add new `Monads` like:

- [Try< T >](https://static.javadoc.io/io.vavr/vavr/0.9.2/io/vavr/control/Try.html)
- [Either< L ,R >](https://static.javadoc.io/io.vavr/vavr/0.9.2/io/vavr/control/Either.html)

Or you could use new ones from Reactor to model your Reactive problems:

- [Mono< T >](https://projectreactor.io/docs/core/release/api/reactor/core/publisher/Mono.html)
- [Flux< T >](https://projectreactor.io/docs/core/release/api/reactor/core/publisher/Flux.html)

The following problems was designed to improve your skills modeling solutions.

Enjoy the journey!

Juan Antonio Breña Moral


##  Problems

### Problem 1

``` gherkin 
Feature: Insurance names

Scenario: Consume the APIs in a Happy path scenario
    Given a Person
    When  call the endpoint /insurance/name
    Then  return the name of the insurance
``` 

![](./docs/class-diagram-type-problem1.svg)

## References

- https://docs.oracle.com/javase/8/docs/api/java/lang/package-summary.html
- https://www.baeldung.com/java-primitives-vs-objects
- [Optional - The Mother of All Bikesheds by Stuart Marks](https://www.youtube.com/watch?v=Ej0sss6cq14)
- https://github.com/aol/cyclops
- https://github.com/vavr-io/vavr
- https://projectreactor.io/docs/
- https://mermaidjs.github.io/mermaid-live-editor/
- https://mermaidjs.github.io/#/classDiagram
- https://www.manning.com/books/java-8-in-action