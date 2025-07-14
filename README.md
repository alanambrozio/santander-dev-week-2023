# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes

```mermaid
classDiagram
  class User {
    +String name
  }

  class Account {
    +String number
    +String agency
    +String balance
    +String limit
  }

  class Feature {
    +String icon
    +String description
  }

  class Card {
    +String number
    +Float limit
  }

  class News {
    +String icon
    +String description
  }

  User --> Account : has
  User --> Card : has
  User --> "0..*" Feature : has
  User --> "0..*" News : has
```
