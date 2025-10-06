```mermaid
graph TD
A([Start])
B[/Input Character ch/]
C{ch is 'a' or 'A'?}
D{ch is 'e' or 'E'?}
E{ch is 'i' or 'I'?}
F{ch is 'o' or 'O'?}
G{ch is 'u' or 'U'?}
H[/Output Vowel/]
I[/Output Consonant/]
J([End])

A --> B
B --> C

C -- Yes --> H
C -- No --> D

D -- Yes --> H
D -- No --> E

E -- Yes --> H
E -- No --> F

F -- Yes --> H
F -- No --> G

G -- Yes --> H
G -- No --> I

H --> J
I --> J
