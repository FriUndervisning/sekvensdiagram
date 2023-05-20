```mermaid
sequenceDiagram
    participant User
    participant PLC

    User->>PLC: Tryk på S1
    Note right of PLC: Tilstand 1
    PLC->>PLC: Aktiver Q1
