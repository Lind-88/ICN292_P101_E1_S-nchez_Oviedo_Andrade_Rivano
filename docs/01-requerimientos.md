#Requerimientos
## Actores y roles 
El encargado es el actor principal ya que el sistema estara diseñado para el. Es quien ingresa la informacion de compras y gastos, y tambien quien consulta la informacion final para tomar las decisiones del negocio.
El cajero es el empleado que atiende el local. Su rol dentro del istema es ingresar las ventas diarias al termino de su jornada.
n8n es un actor extermo que extrae la informacion del sistema y la usa para asistir, por ejemplo enviando correos o recomendaciones.
## Alcance in / out 
1) Resgistro de ventas: esta dentro del alcance registrar las ventas totales diarias segregadas por metodo de pago, no estara dentro del alcance registrar cada venta en particular, esto es, no habra un analisis de productos mas vendidos (falta de punto de venta y capacidad de discriminacion)
2) Registro de compra a proveedores: Esta dentro del alcance registrar el monto total de la factura y su fecha. No se registran los poductos especificos comprados, ni sus precios ni cantidades.
3) Analisis de indicadores: esta dentro del alcance calcular indicadores como ventas mensuales, compras a proveedores y gastos promedio. Queda fuera del alcance calcular indicadores como margen de ventar por producto o producto comprado mas frecuentemente.
4) Automatizacion de pan: esta dentro del alcance registrar la compra y el stock de pan y generar una recomendacion de la cantidad a abastecer, queda fuera del alcance realizar la compra automatica.
5) Notificaciones automaticas: Esta dentro del alcance enviar notificaciones por telegram al encargado para recordarle los registros diarios. Queda fuera del alcance enviar mensajes automaticos a proveedores, clientes o aplicaciones externas.

##Requisitos funcionales
1) El sistema debe registrar las ventas diarias, con el monto total y los montos desagregados por el metodo de pago (must have)
2) El sistema debe registrar las compras a proveedores, considerando fecha, proveedor, monto y metodo de pago. (must have)
3) El sistema debe permitir crear, editar y consultar proveedores, categorias y medios de pago. (must have)
4) El sistema debe permitir consultar y busccar informacion en los datos historicos. (must have)
5) El sistema debe permitir crear, editar y consultar proveedores, categorias y medios de pago. (must have)
6) El sistema debe calcular indicadores de desempeño del periodo. (must have)
7) El sistema debe recordar al encargado realizar los registros diarios. (should have)
8) El sistema debe registrar la cantidad de pan abastecido y el stock disponible. (should have)
9) el sistema debe recomendar al encargado la cantidad de pan a abastecer. (should have)

El primer problema es sobre el registro manual y la dificultad de consolidarlo, se atiende con los requisitos 1, 2 y 3, el 5 y el 6

El segundo problema sobre los registros incompletos y la perdida de informacion se atiende con los requisitos 1, 2, 3, 7

El tercer problema se atiende con los requisitos 5 y 6, que permiten que el encargado decida con informacion y no solo con criterio propio.

El cuarto problema, sobre la falta de registro de inventario y el abastecimiento por herramientas por observacion se atiende con los 8 y 9, que entregan al encargado mas herramientas para decidir cuanto pan comprar.

##Requisimos no funcionales
1) El sistema debe ser sencillo de aprender para cualquiera (must have)
2) El sistema debe guardar la informacion de manera permanente, de modo que siga disponible en los proximos usos. (must have)
3) El sistema debe permitir que los usuarios sin conocimientos tecnicos modifiquen categorias y medios de pago. (must have)
4) El sistema debe permitir realizar los registros diarios en un bajo numero de pasos. (must have)
5) El sistema debe garantizar que la informacion ingresada cumpla los formatos definidos. (must have)
6) El sistema debe presentar los indiadores de desempeño de forma clara y compresnible para la toma de decisiones. (must have)

El primer problema se atiende facilitando el registro con pocos pasos (4), almacenando la informacion de forma permanente (2) y presentando los indicadores de manera clara (6).

El segundo problema se atiende asegurando que los usuarios no necesiten conocimientos especializados (1 y 3), que el registro sea rapido (4) y que la informacion se mantenga entre sesiones (2)

El tercer problema se atiende guardando la informacion de forma permanente (2) y mostrandola de forma clara y util para decidir (6).

El cuarto problema se atiende con un sistema fácil de aprender (1), con pocos pasos (4) y con validación de los datos ingresados (5), para que el encargado pueda consultar después esa información y decidir de manera informada.






