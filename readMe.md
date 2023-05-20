```mermaid
sequenceDiagram
    participant User
    participant PLC
    participant Tegnestandard

    User->>PLC: Tryk på S1
    Note right of PLC: Tilstand 1
    PLC->>PLC: Skift til Tilstand 2
    Note over PLC: DS/EN 61131-3

    User->>PLC: Tryk på S2
    Note right of PLC: Tilstand 2
    PLC->>PLC: Skift til Tilstand 3
    Note over PLC: DS/EN 61131-3

    User->>PLC: Tryk på S3
    Note right of PLC: Tilstand 3
    PLC->>PLC: Skift til Tilstand 4
    Note over PLC: DS/EN 61131-3

    User->>PLC: Tryk på S4
    Note right of PLC: Tilstand 4
    PLC->>PLC: Skift til Tilstand 1
    Note over PLC: DS/EN 61131-3

    PLC->>Tegnestandard: Følg DS/EN 61131-3
