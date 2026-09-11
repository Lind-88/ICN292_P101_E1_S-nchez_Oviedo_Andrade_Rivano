## ER Preliminar.
Las entidades del ER preliminares son:
# Ventas diarias:
Caracteristicas: Fecha (PK), Monto total, Monto crédito, Monto débito y Monto efectivo.
# Compras Proveedores:
Caracteristicas: ID de la factura (PK), Monto total, Fecha y Rut proveedor (FK).
# Proveedor:
Características: Rut del proveedor (PK) y Nombre del proveedor.
# Flujo de Pan:
Características: Fecha (PK), Pan comprado y Stock actual de pan. 
# Gasto operacional:
Características: ID Gasto (PK), Fecha, Monto total, ID Categoría (FK).
# Tipo de Gasto:
Características: ID Categoría (PK) y Nombre Categoría.

## Cardinalidad.
Las relaciones entre las entidades se definene de la siguiente manera:
Proveedores <- 1:N -> Compras Proveedores
Muchas Compras a Proveedores pueden estar asociadas a un Proveedor.

Tipos de Gasto <- 1:N -> Gastos Operacionales
Muchos Gastos pueden estar asociados a un Tipo de Gasto.

## Trazabilidad.
El modelo ER permite almacenar la informacón generada durante el proceso BPMN To-Be:

Ventas diarias: se genera a partir del ingreso de información por parte del cajero al realizar el cierre de caja.
Compas a proveedores y Proveedores: son respaldadas por las tareas realizadas por el encargado al abasteser e ingresar los datos
Flujo de Pan: es sostenido por el encargado a la hora de realizar el abastecimiento de pan.
Gastos Operacionales: esta entidad es respaldada por el encargado, ya que es este el que realiza el registro de los gastos operacionales.

