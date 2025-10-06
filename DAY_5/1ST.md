```mermaid
graph TD
A([Start])
B[/Input num1, op, num2/]
C{op?}
D{op == '+'?}
E{op == '-'?}
F{op == '*'?}
G{op == '/'?}
H[result = num1 + num2]
I[result = num1 - num2]
J[result = num1 * num2]
K{num2 != 0?}
L[result = num1 / num2]
M[/Output result/]
N[/Output "Division by zero" Error/]
O[/Output "Invalid operator" Error/]
P([End])

A --> B
B --> D

D -- Yes --> H
H --> M

D -- No --> E
E -- Yes --> I
I --> M

E -- No --> F
F -- Yes --> J
J --> M

F -- No --> G
G -- Yes --> K
G -- No --> O

K -- Yes --> L
L --> M
K -- No --> N

M --> P
N --> P
O --> P
