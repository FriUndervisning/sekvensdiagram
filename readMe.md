```mermaid
stateDiagram-v2
    Tilstand1: Tilstand 1
    Tilstand1: Udgående besked, linje 1
    Tilstand1: Udgående besked, linje 2
    [*] --> Tilstand1
    Tilstand1 --> Tilstand2 : S1
    Tilstand2: Indgående besked
    Tilstand2: Udgående besked, linje 1
    Tilstand2: Udgående besked, linje 2
    Tilstand2 --> Tilstand3 : S2
    Tilstand3: Indgående besked
    Tilstand3: Udgående besked, linje 1
    Tilstand3: Udgående besked, linje 2
    Tilstand3 --> Tilstand4 : B3
    Tilstand4: Indgående besked
    Tilstand4: Udgående besked, linje 1
    Tilstand4: Udgående besked, linje 2
    Tilstand4 --> Tilstand1 : S3




