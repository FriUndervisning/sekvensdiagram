```mermaid
sequenceDiagram
    Participant User
    Participant System

    User->>System: Request
    activate System
    System-->>User: Response
    deactivate System
