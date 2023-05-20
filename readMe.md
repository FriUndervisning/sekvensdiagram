```mermaid
sequenceDiagram
    participant User
    participant System

    User->>System: Send anmodning

    alt Anmodning godkendt
        System->>System: Valider anmodning
        System->>System: Behandle anmodning
        System->>User: Send svar
    else Anmodning afvist
        System->>User: Send afvisningssvar
    end

    loop Gentagne handlinger
        System->>System: Udfør handling
    end

    opt Optimeret handling
        System->>System: Udfør hurtig handling
    end

    par Fragmenteret handling
    par A
        User->>System: Send anmodning A
        System->>User: Send svar A
    end
    par B
        User->>System: Send anmodning B
        System->>User: Send svar B
    end
    end

    User->>System: Afslut anmodning
