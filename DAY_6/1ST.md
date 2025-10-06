```mermaid
graph TD
A([Start])
B[/Input N/]
C[i = 1]
D{i <= 10?}
E[Product = N * i]
F[/Output N x i = Product/]
G[i = i + 1]
H([End])

A --> B
B --> C
C --> D
D -- Yes --> E
E --> F
F --> G
G --> D
D -- No --> H
