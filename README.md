# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev week 

## Diagrama de Classes

```mermaid
classDiagram
class User {
  - name: string
  - account: Account
  - feature: Features[]
  - card: Card
  - news: News
}

class Account {
  - number: string
  - agency: string
  - balance: number
  - limit: number
}

class Feature {
  - Icon: string
  - description: string
}

class Card {
  - Number: string
  - Limit: number
}

class News {
  - Icon: string
  - description: string
}

User "1" *-- "1" Account
User "1" *-- "N" Feature
User "1" *-- "1" Card
User "1" *-- "N" News
```
