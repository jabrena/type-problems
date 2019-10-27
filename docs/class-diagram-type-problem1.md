# Class diagram for Type problem 1

- https://mermaidjs.github.io/mermaid-live-editor

## Diagram:

```
classDiagram
      Person *-- Car
      Car *-- Insurance
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
