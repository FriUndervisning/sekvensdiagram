```mermaid
sequenceDiagram
    participant User
    participant PLC

    User->>PLC: Tryk på S1

    PLC->>PLC: Skift til Tilstand 2
    Note over PLC: Tilstand 1

    User->>PLC: Tryk på S2

    PLC->>PLC: Skift til Tilstand 3
    Note over PLC: Tilstand 2

    User->>PLC: Tryk på S3

    PLC->>PLC: Skift til Tilstand 4
    Note over PLC: Tilstand 3

    User->>PLC: Tryk på S4

    PLC->>PLC: Skift til Tilstand 1
    Note over PLC: Tilstand 4
