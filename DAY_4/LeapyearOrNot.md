
```mermaid
graph TD
A([Start])
B[/Input Year/]
C{Year % 400 == 0?}
D{Year % 100 == 0?}
E{Year % 4 == 0?}
F[/Output Leap Year/]
G[/Output NOT a Leap Year/]
H([End])

A --> B
B --> C

C -- Yes --> F
F --> H

C -- No --> D

D -- Yes --> G
G --> H

D -- No --> E

E -- Yes --> F
E -- No --> G
