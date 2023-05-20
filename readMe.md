```mermaid
stateDiagram-v2
    Tilstand1: Tilstand 1
    Tilstand1: M1 := 0 <br>Grøn lampe blink := 0<br>Grøn lampe konstant := 0 <br>Drift produktion := 0
    [*] --> Tilstand1
    Tilstand1 --> Tilstand2 : S1
    Tilstand2: Tilstand 2
    Tilstand2: M1 := 1 <br>Grøn lampe blink := 1
    Tilstand2 --> Tilstand3 : S2
    Tilstand3: Tilstand 3
    Tilstand3: Grøn lampe blink := 0<br>Grøn lampe konstant := 1
    Tilstand3 --> Tilstand4 : B3
    Tilstand4: Tilstand 4
    Tilstand4: Drift produktion := 1
    Tilstand4 --> Tilstand1 : S3


