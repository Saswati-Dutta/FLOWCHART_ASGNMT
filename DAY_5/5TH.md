```mermaid
graph TD
A([Start])
B[/Input Marks/]
C[Calculate m]
D{Check Range}
E{Check A+}
F[Set A+]
G[Set A]
H[Set B]
I[Set C]
J[Set F]
K[/Output Grade/]
L([End])

A --> B
B --> C
C --> D
D -- 10 or 9 --> E
E -- Yes --> F
E -- No --> G
D -- 8 --> H
D -- 7 --> I
D -- Default --> J

F --> K
G --> K
H --> K
I --> K
J --> K
K --> L
