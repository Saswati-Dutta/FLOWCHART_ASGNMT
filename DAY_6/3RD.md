```mermaid
graph TD
A([Start])
B[/Input N/]
C[Init Fact]
D{N Negative?}
E[/Error/]
F[Init I]
G{Loop End?}
H[Update Fact]
I[Increment I]
J[/Output Fact/]
K([End])

A --> B
B --> C
C --> D
D -- Yes --> E
E --> K
D -- No --> F
F --> G
G -- Yes --> H
H --> I
I --> G
G -- No --> J
J --> K
