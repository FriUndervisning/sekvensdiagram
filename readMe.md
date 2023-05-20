sequenceDiagram
    participant Sensor
    participant PLC
    participant Motor

    Sensor->>PLC: Indgangssignal detekteret
    PLC->>Motor: Aktiver motor
    PLC->>Sensor: Kontroller motorstatus
