```mermaid
graph TD
A([Start])
B[/Input Total Units/]
C[/Input Choice/]
D{Choice?}
E[Calculate First 100]
F[Calculate Next 100]
G[Calculate Above 200]
H{Units <= 100?}
I{Units <= 200?}
J[Calculate Tier 1 Total]
K[Calculate Tier 1 + 2 Total]
L[Calculate All Tiers Total]
M[/Output Bill/]
N[/Output Invalid choice Error/]
O([End])

A --> B
B --> C
C --> D
D -- Case 1 --> E
E --> M
D -- Case 2 --> F
F --> M
D -- Case 3 --> G
G --> M

D -- Case 4 --> H
H -- Yes --> J
J --> M
H -- No --> I
I -- Yes --> K
K --> M
I -- No --> L
L --> M

D -- Default --> N

M --> O
N --> O
