# Class diagram for Type problem 1

- https://mermaidjs.github.io/mermaid-live-editor

## Diagram:

```
classDiagram
      Person *-- "0..1" BeachHouse
      BeachHouse *-- "0..1" Insurance
      class Person {
          -BeachHouse house
          +getHouse()
      }
      class BeachHouse {
          -Insurance insurance
          +getInsurance()
      }
      class Insurance {
          - String name
          +getName()
      }
```

## Visualization:

![](./class-diagram-type-problem1.svg)

## Config:

```
{
  "theme": "forest"
}
```
