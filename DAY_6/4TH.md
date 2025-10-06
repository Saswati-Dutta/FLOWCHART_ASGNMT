```mermaid
graph TD
A([Start])
B[/Input N/]
C[Init First=0, Second=1]
D[i = 1]
E{i <= N?}
F[/Output First/]
G[Next = First + Second]
H[First = Second]
I[Second = Next]
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
