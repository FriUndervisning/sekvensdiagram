```mermaid
stateDiagram-v2
    Tilstand1: Tilstand 1
    Tilstand1: Tænd M1
    [*] --> Tilstand1
    Tilstand1 --> Tilstand2 : S1
    Tilstand2: Indgående besked
    Tilstand2: Udgående besked
    Tilstand2 --> Tilstand3 : S2
    Tilstand3: Tilstand 3
    Tilstand3: Sluk M1
    Tilstand3 --> Tilstand4 : B3
    Tilstand4: Indgående besked
    Tilstand4: Udgående besked
    Tilstand4 --> Tilstand1 : S3


