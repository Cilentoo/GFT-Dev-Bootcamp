# GFT- DEV BOOTCAMP
Java RESTful API criada de replicada para entrega de projeto final no GFT BOOTCAMP JAVA COM IA
RESTful Java API created and replicated for final project delivery in GFT BOOTCAMP JAVA WITH AI

## Diagrama de classes (Class Diagram)

```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +Feature[] features
        +Card card
        +News[] news
    }

    class Account {
        +String number
        +String agency
        +double balance
        +double limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +double limit
    }

    class News {
        +String icon
        +String description
    }

    User "1" *-- "1" Account
    User "1" *-- "0..*" Feature
    User "1" *-- "1" Card
    User "1" *-- "0..*" News
```
