flowchart TD
    subgraph STOCK[Gestión de Stock]
        Compras[Compras de origen] --> Inventario[Seguimiento Inventario]
    end

    subgraph VENTAS[Gestión de Ventas]
        VentasX[Ventas X país] --> Comisiones
        VentasY[Ventas Y país] --> Comisiones
        VentasZ[Ventas Z país] --> Comisiones
    end

    subgraph CLIENTES[Gestión de Clientes]
        VentasX --> SeguimientoClientes[Seguimiento de Clientes]
        VentasY --> SeguimientoClientes
        VentasZ --> SeguimientoClientes
    end

    Inventario --> Comisiones
    Inventario --> SeguimientoClientes
