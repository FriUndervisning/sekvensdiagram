```mermaid
    stateDiagram-v2
    [*] --> Tilstand1
    Tilstand1 --> Tilstand2 : handling1
    Tilstand2 --> Tilstand3 : handling2
    Tilstand3 --> Tilstand4 : handling3
    Tilstand4 --> [*] : handling4

