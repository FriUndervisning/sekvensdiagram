```mermaid
stateDiagram-v2
    [*] --> Tilstand1
    Tilstand1 --> Tilstand2 :     S1     
    Tilstand2 --> Tilstand3 :     S2     
    Tilstand3 --> Tilstand4 :     B3     
    Tilstand4 --> Tilstand1 :     S3     

