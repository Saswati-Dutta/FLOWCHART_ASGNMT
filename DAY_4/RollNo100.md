
```mermaid
graph TD
A([Start])
B[/Input Roll Number/]
C{roll == 100?}
D{roll != 100?}
E[/Output "100 is present."/]
F[/Output "100 is not present."/]
G([End])

A --> B
B --> C
B --> D

C -- Yes --> E
D -- Yes --> F

E --> G
F --> G
