```mermaid
graph TD
A([Start])
B[/Input N/]
C[sum = 0]
D[i = 1]
E{i <= N?}
F[sum = sum + i]
G[i = i + 1]
H[/Output Sum/]
I([End])

A --> B
B --> C
C --> D
D --> E
E -- Yes --> F
F --> G
G --> E
E -- No --> H
H --> I
