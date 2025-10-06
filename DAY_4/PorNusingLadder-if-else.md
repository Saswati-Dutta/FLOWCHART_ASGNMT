

```mermaid
graph TD
A([Start])
B[/Input num/]
C{num > 0?}
D{num < 0?}
E[/Output Positive/]
F[/Output Negative/]
G[/Output Zero/]
H([End])

A --> B
B --> C

C -- Yes --> E
E --> H

C -- No --> D

D -- Yes --> F
F --> H

D -- No --> G
G --> H
