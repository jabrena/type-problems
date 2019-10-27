# Class diagram for Type problem 1

- https://mermaidjs.github.io/mermaid-live-editor

## Diagram:

```
classDiagram
classDiagram
      Person "1" --> "0..1" Car
      Car "1" --> "0..1" Insurance
      class Person {
          -Car car
          +getCar()
      }
      class Car {
          -Insurance insurance
          +getInsurance()
      }
      class Insurance {
          - String name
          +getName()
      }
```

## Visualization:

![](./sequence-diagram-latency-problem1.svg)

## Config:

```
{
  "theme": "forest"
}
```
