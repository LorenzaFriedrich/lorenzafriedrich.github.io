graph TB
    subgraph "CLIENT SIDE"
        A["gfclient.c<br/><br/>YOU IMPLEMENT"]
        B["gfclient.h<br/><br/>Interface Definition"]
        C["gfclient_download.c<br/><br/>Test Program"]
        D["workload.h/c<br/><br/>Workload Manager"]
        
        C --> |uses| A
        A --> |implements| B
        C --> |reads| D
    end
    
    subgraph "PROTOCOL"
        E["GETFILE Protocol<br/><br/>TCP Communication"]
        F["Request Format:<br/>GETFILE GET /path\\r\\n\\r\\n"]
        G["Response Format:<br/>GETFILE status length\\r\\n\\r\\n data"]
    end
    
    subgraph "SERVER SIDE"
        H["gfserver.c<br/><br/>YOU IMPLEMENT"]
        I["gfserver.h<br/><br/>Interface Definition"]
        J["gfserver_main.c<br/><br/>Test Program"]
        K["content.h/c<br/><br/>File Manager"]
        L["handler.o<br/><br/>Request Handler"]
        
        J --> |uses| H
        H --> |implements| I
        H --> |callbacks| L
        L --> |gets files| K
    end
    
    %% Network connection
    A -.-> |network| E
    E -.-> |network| H
    
    style A fill:#ffcdd2
    style H fill:#ffcdd2
    style E fill:#e1f5fe