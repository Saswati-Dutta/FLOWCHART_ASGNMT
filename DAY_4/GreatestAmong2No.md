```mermaid
graph TD
A([Start])
B[/Input a, b/]
C{a > b?}
D{b > a?}
E[/Output a is greater/]
F[/Output b is greater/]
G[/Output Both are equal/]
H([End])

A --> B
B --> C
C -- Yes --> E
C -- No --> D
D -- Yes --> F
D -- No --> G
E --> H
F --> H
G --> H
