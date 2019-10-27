# Class diagram for Type problem 1

- https://mermaidjs.github.io/mermaid-live-editor

## Diagram:

```
classDiagram
      Person *-- "0..1" BeachHouse
      BeachHouse *-- "0..1" Insurance
      class Person {
          -BeachHouse house
          +Person(BeachHouse house)
          +BeachHouse getHouse()
      }
      class BeachHouse {
          -Insurance insurance
          +BeachHouse(Insurance house)
          +Insurance getInsurance()
      }
      class Insurance {
          -String name
          +Insurance(String name)
          +String getName()
      }
      class TypeProblem1 {
          -String DEFAULT_FALLBACK = "Not available"
          -Person person
          +TypeProblem1(Person person)
          +String getInsuranceName()
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
