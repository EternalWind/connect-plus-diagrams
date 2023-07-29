```mermaid
sequenceDiagram
    Creator->>Creator: generate key pair for the forum and store them
    Creator->>+Server: send the forum's information with its pk
    Server->>Server: store the forum's information and pk
    Server->>Server: grant the created forum's ownership to Creator
    Server-->>-Creator: acknowledge
```