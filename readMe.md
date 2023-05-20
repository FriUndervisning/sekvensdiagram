```mermaid
stateDiagram-v2
    Tilstand1: M1 := 0 
    Tilstand1: Gron lampe blink := 0
    [*] --> Tilstand1
    Tilstand1 --> Tilstand2 : S1
    Tilstand2: Indgående besked
    Tilstand2: Udgående besked
    Tilstand2 --> Tilstand3 : S2
    Tilstand3: Indgående besked
    Tilstand3: Udgående besked
    Tilstand3 --> Tilstand4 : B3
    Tilstand4: Indgående besked
    Tilstand4: Udgående besked
    Tilstand4 --> Tilstand1 : S3



