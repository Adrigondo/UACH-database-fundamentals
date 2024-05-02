# Practica Caso de estudio #1
### Analisis de la información
Se recabo la información de las siguientes entidades.
- **Usuarios**. Identificador(codigoUsuario), dni, telefono fijo, telefono movil, nombre, apellidos.
- **Cliente**. Identificador(codigoPersonal),  relacion(codigoUsuario).
- **Trabajadores**. Identificador(codigoTrabajador), relacion(codigoUsuario), relacion(codigoPersonal).
- **Datos de inmuebles**. Identificador(codigoDeDatosDeInmueble), area (m^2), descripcion, direccion.
- **Pisos**. Identificador(codigoDePiso), relacion(codigoDeDatosDeInmueble).
- **Locales**. Identificador-Relacion(codigoDeDatosDeInmueble), uso, ¿hay servicio?.
- **Garajes**. Identificador(codigoDeGaraje), relacion(codigoDeDatosDeInmueble), planta, relacion(codigoDePiso)
- **Otros inmuebles**. Identificador(codigoDeInmueble),  relacion(codigoDeDatosDeInmueble).
- **Compra**. Identificador(codigoCompra), relacion(codigoDeDatosDeInmueble), relacion(codigoPersonal), fecha, monto.
    - Relación muchos a muchos entre clientes y compras. Relacion(codigoPersonal), relacion(codigoCompra).
- **Alquileres**. Identificador(idAlquiler), numero de alquiler, relacion(codigoDeDatosDeInmueble), relacion(codigoPersonal), relacion(codigoTrabajador).
- **Pagos**. Identificador(idAlquiler), año, mes, monto.