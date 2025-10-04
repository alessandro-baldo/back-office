```mermaid
  graph TD;
	graph LR
    subgraph STOCK[Gestión de Stock]
        A[Compras de origen]
        G[Seguimiento Inventario]
    end

    subgraph VENTAS[Gestión de Ventas]
        B[Ventas X país]
        C[Ventas Y país]
        D[Ventas Z país]
    end

    subgraph RESULTADOS[Resultados]
        E[Comisiones]
        F[Seguimiento Clientes]
    end

    A --> G
    B --> E
    C --> E
    D --> E
    B --> F
    C --> F
    D --> F
    B --> G
    C --> G
    D --> G

```