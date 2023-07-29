```mermaid
sequenceDiagram
    Sender->>+Server: send chat message encrypted with forum's pk
    Server-->>-Sender: acknowledge
    Server->>+Recipient: forward encrypted chat message
    Recipient->>Recipient: decrypt chat message with forum's ppk
    Recipient-->>-Server: acknowledge
```