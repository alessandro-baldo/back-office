```mermaid

flowchart LR
    subgraph Ingreso de datos
        A[Compras de origen]
        B[Ventas X país]
        C[Ventas Y país]
        D[Ventas Z país]
        E[Pagos a proveedores]
    end

    subgraph Salida de datos
        F[Seguimiento de inventario]
        G[Seguimiento de clientes]
        H[Seguimiento de comisiones]
        I[Seguimiento a proveedores]
    end

    subgraph Reportes
        J[Reporte de ventas]
        K[Reporte de inventario]
        L[Reporte de compras]
    end

    A --> F
    B --> F
    C --> F
    D --> F

    B --> G
    C --> G
    D --> G

    B --> H
    C --> H
    D --> H

    E --> I

    F --> K
    G --> J

    I --> L
\```
