```mermaid
graph TD
A([Start])
B[/Input num/]
C{num % 2 == 0?}
D[/Output Even/]
E[/Output Odd/]
F([End])

A --> B
B --> C
C -- Yes --> D
C -- No --> E
D --> F
E --> F
