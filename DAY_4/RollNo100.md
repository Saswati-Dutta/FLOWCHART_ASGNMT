
```mermaid
graph TD
A([Start])
B[/Input a, b, c/]
C{a > b?}
D{a > c?}
E{b > c?}
F[/Output a is Max/]
G[/Output b is Max/]
H[/Output c is Max/]
I([End])

A --> B
B --> C

C -- Yes --> D
D -- Yes --> F
D -- No --> H
F --> I
H --> I

C -- No --> E
E -- Yes --> G
E -- No --> H
G --> I
