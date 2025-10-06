
```mermaid
graph TD
    a([Start])
    b[Input Choice]
    c{Choice is 1?}
    d{Choice is 2?}
    e[Input C]
    f[Calculate F]
    g[Output F]
    h[Input F]
    i[Calculate C]
    j[Output C]
    k[Invalid Choice]
    l([End])
    
    a --> b
    b --> c
    
    c -- Yes --> e
    e --> f
    f --> g
    
    c -- No --> d
    
    d -- Yes --> h
    h --> i
    i --> j
    
    d -- No --> k
    
    g --> l
    j --> l
    k --> l
