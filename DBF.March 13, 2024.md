# Reporte de caso 2
Una compañía de transporte recoge pedidos de los almacenes de una cadena y los entrega a las tiendas de la misma cadena.
- Actualmente hay 6 almacenes y 45 tiendas. Cada tienda tiene su propio nombre, y conocemos también su dirección y teléfono. Cada almacén tiene un número diferente además de la dirección y teléfono.
- Un camión puede transportar varios pedidos en el mismo viaje y entregar cada pedido a la tienda que lo solicito.
- Cada viaje se identifica por un número. Cada pedido se identifica por un número e incluye datos sobre peso, volumen y tienda de destino.
- Cada camión tiene el número de matrícula y su propio límite máximo de volúmenes y peso trasportado.

La flota de la compañía de transporte consta de 150 vehículos y cada uno realiza entre 3 y 4 viajes semanales.

Esta base de datos la usarán conjuntamente las dos empresas para:
1.	Controlar el uso de los camiones (fechas).
2.	Controlar las entregas (pedidos entregados)
3.	Programar

Se solicita realizar el modelo Entidad-Relacional(o bien modelo MEER) y a partir de ese modelo realizar el modelo Relacional

## Analisis
- Tiendas: identificador(nombre), dirección, teléfono
- Almacenes: identificador(número), dirección, teléfono
- Camiones: identificador(número de matrícula), límite de volumen máximo, límite de peso máximo
- Viajes: identificador(número), fecha de salida, fecha de llegada, relación(camión)
- Pedidos: identificador(número), peso, volumen,relación(tienda), relación(viaje), estatus.
 
