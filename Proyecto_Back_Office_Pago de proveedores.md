## Proyecto <Back Office>

## Seguimiento de pagos a proveedores

Objetivo
Tener a disposición datos actualizados sobre los pagos realizados y documentación recibida, por cliente.
Conciliación de pagos.

//

## Estructura de las planillas a usar:

1. Planilla general de pagos (colaborativa):
- Se ingresa manualmente la información de la documentación a pagar.
- Columnas estructuradas (Emisión, Proveedor, RUT, Moneda, Monto, Estado del pago).
- Uso de forma colaborativa para el seguimiento de pagos.

2. Planilla del sistema de facturación (individual):
- Se descarga directamente del sistema de facturación (reporte compras) 
- Se actualiza de forma periódica.

3. Planilla de conciliación de pagos (individual)
- Se importa la planilla colaborativa a traves de la función "importrange".
- Cruzar información a traves del numero de RUT.

//

## Uso de la planilla:
1. Importar la planilla general de pagos usando "IMPORTRANGE"
2. Actualizar manualmente los datos del sistema de facturación.
3. A traves de la función "FILTER" cruzar datos usando de referencia el numero de RUT.
4. Seleccionar periodo.
5. Revisar diariamente y conciliar.

## Fórmulas útiles:
1. IMPORTRANGE
2. FILTER

//

Comentarios finales:

Permite la conciliación entre los pagos realizados y la documentación recibida, filtrando por cliente y periodo de emisión.


