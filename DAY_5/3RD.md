```mermaid
graph TD
A([Start])
B[/Input Basic Salary/]
C[/Input Choice/]
D{Choice?}
E[hra = 2.0 * basic]
F[ta = 0.10 * basic]
G[da = 0.05 * basic]
H[Calc all components]
I[gross = basic + hra + ta + da]
J[/Output HRA/]
K[/Output TA/]
L[/Output DA/]
M[/Output Gross Salary/]
N[/Output Invalid choice Error/]
O([End])

A --> B
B --> C
C --> D
D -- Case 1 --> E
E --> J
D -- Case 2 --> F
F --> K
D -- Case 3 --> G
G --> L
D -- Case 4 --> H
H --> I
I --> M
D -- Default --> N

J --> O
K --> O
L --> O
M --> O
N --> O
