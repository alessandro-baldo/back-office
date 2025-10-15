```mermaid

flowchart LR

%% Ingresos de datos

    subgraph Ingreso de datos
        A[Compras de origen];
        B[Ventas X país];
        C[Ventas Y país];
        D[Ventas Z país];
        E[Pagos a proveedores];
    end

%% Procesamiento de datos

    subgraph Procesamiento de datos
        F[Seguimiento de inventario];
        G[Seguimiento de clientes];
        H[Seguimiento de comisiones];
        I[Seguimiento a proveedores];
    end

%% Reportes

    subgraph Reportes
        J[Reporte de ventas];
        K[Reporte de inventario];
        L[Reporte de compras];
        M[Reporte de comisiones]  
    end

%% Visualización

    subgraph Visualización
        O[Dashboards]
        P[KPI's] 
    end


%% Primer flujo

    A --> F;
    B --> F;
    C -.-> F;
    D -.-> F;

    B --> G;
    C -.-> G;
    D -.-> G;

    B --> H;
    C -.-> H;
    D -.-> H;

    E --> I;

%% Segundo flujo

    F --> K;
    G --> J;
    H --> M;
    I --> L;

%% Tercer flujo

    K --> P;
    J --> P;
    M --> P;
    L --> P;
    P --> O;

click P "https://github.com/alessandro-baldo/back-office/blob/main/kpis.md"

%% Fin


























