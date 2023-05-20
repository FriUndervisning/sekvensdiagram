```mermaid
sequenceDiagram
    participant User
    participant PLC

    User->>PLC: Tryk på S1
    Note right of PLC: Tilstand 1
    PLC->>PLC: Skift til Tilstand 2

    User->>PLC: Tryk på S2
    Note right of PLC: Tilstand 2
    PLC->>PLC: Skift til Tilstand 3

    User->>PLC: Tryk på S3
    Note right of PLC: Tilstand 3
    PLC->>PLC: Skift til Tilstand 4

    User->>PLC: Tryk på S4
    Note right of PLC: Tilstand 4
    PLC->>PLC: Skift til Tilstand 1
