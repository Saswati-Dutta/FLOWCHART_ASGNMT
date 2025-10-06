```mermaid
graph TD
A([Start])
B[/Input ch/]
C{Is ch a Vowel?}
D{Is ch an Alphabet?}
E[/Output Vowel/]
F[/Output Consonant/]
G[/Output Not Alphabet/]
H([End])

A --> B
B --> C
C -- Yes --> E
C -- No --> D
D -- Yes --> F
D -- No --> G
E --> H
F --> H
G --> H
