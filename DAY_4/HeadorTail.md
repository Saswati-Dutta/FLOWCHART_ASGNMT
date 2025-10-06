
```mermaid
graph TD
A([Start])
B[/Input Coin/]
C{Check for Head?}
D{Check for Tail?}
E[/Output Head Result/]
F[/Output Tail Result/]
G[/Output Invalid/]
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
