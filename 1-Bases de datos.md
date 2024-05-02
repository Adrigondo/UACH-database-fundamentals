¿Para qué nos sirve? Para registrar y representar el funcionamiento de un sistema a traves de sus datos. Un objetivo es proporcionar al final una vista abstracta de los datos proporcionados.
1.	Disminuir redundancia
Es necesario disminuir la posibilidad de que exista redundancia de la información y que etos siempre estén completos. Los campos y atributos sobre esa tabla, son los que requerimos, si no, no hay que ponerlos. 
2.	Evitar el aislamiento de los datos.

3.	Corregir anomalías en el acceso concurrente.
Permisión de que varios usuarios actualicen la información simultánieamente.
4.	Disminuir problemas de seguridad
No es recomendable que todos los usuarios de la base de dartos tengan acceso a toda la información de todos los datos. Nosotros debemos designar que información estará disponible apra que roles, definir los limites entre estos datos.
5.	Disminuir los problemas de integridad
Deben satisfacer ciertos tipos de limitantes de consistencia:
-	Acceso concurrente por parte de múltiples usuarios.
-	Integridad de los datos.
-	Consultas complejas optimizadas.
-	Seguridad de acceso y auditoría.
-	Respldo y recuperación.
-	Acceso a través de lengujae de programación estándar.

## Áreas de aplicación de los sistemas de bases de datos
Bancos escuelas, finanzas, telecomunicaciones, streaming, etc. Actualmente todo tiene una base de datos.

## Modelos de datos
Un modelo de datos determina la estructura lógica de una base de datos y determina el modo de almacenar, organizar y manipular datos.
Los modelos lógicos de datos:
- Modelo jerárquico
- Modelo en r3d
- Modelo relacional
- Modelo entidad-relación
- Modelo entidad-relación-extendido
- Modelo de objetos
- Modelo documental
- Modelo entidad-atributo-valor
- Modelo en estrella
Los modelos físicos de datos:
- Indice invertido
- Fichero plano
El modelo relacional de datos fue introducido en 1970 pot Codd con el objetivo de querer hacer los SGBD más independientes de las aplicaciones. Modelo matemático definido en terminos de lógica de prredicados y teoría de conjuntos.

El Sistema Gestor nos sirve para crear una base de datos.

# DDL (Data Definition Language)
# DML (Data Manipulation Language)