```mermaid
graph TD
A([Start])
B[/Input N/]
C[Init F=0, S=1]
D[i = 1]
E{i <= N?}
F[/Output F/]
G[Next = F + S]
H[F = S]
I[S = Next]
J[i = i + 1]
K([End])

A --> B
B --> C
C --> D
D --> E
E -- Yes --> F
F --> G
G --> H
H --> I
I --> J
J --> E
E -- No --> K
