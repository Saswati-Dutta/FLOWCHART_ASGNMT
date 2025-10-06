```mermaid
graph TD
A([Start])
B[/Input a, b, c/]
C[D = b*b - 4*a*c]
D{D > 0?}
E{D == 0?}
F[root1, root2 = Real & Different]
G[root1, root2 = Real & Equal]
H[Calculate Real & Imaginary Parts]
I[/Output Real & Different Roots/]
J[/Output Real & Equal Roots/]
K[/Output Complex Roots/]
L([End])

A --> B
B --> C
C --> D

D -- Yes --> F
F --> I
I --> L

D -- No --> E

E -- Yes --> G
G --> J
J --> L

E -- No --> H
H --> K
K --> L
