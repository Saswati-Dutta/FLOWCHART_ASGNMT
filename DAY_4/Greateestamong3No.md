```mermaid
graph TD
A([Start])
B[/Input a, b, c/]
C{a > b AND a > c?}
D{b > a AND b > c?}
E{c > a AND c > b?}
F[/Output a is greatest/]
G[/Output b is greatest/]
H[/Output c is greatest/]
I[/Output Equal or Tied/]
J([End])

A --> B
B --> C

C -- Yes --> F
F --> J

C -- No --> D

D -- Yes --> G
G --> J

D -- No --> E

E -- Yes --> H
H --> J

E -- No --> I
I --> J
