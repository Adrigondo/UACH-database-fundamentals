```sql
create database temp;
use temp;
drop table agenda;
create table agenda
(
    id int unsigned zerofill primary key not null,
    nombre varchar(45) not null,
    apellido_paterno varchar(45) not null,
    apellido_materno varchar(45),
    rfc varchar(13) unique  not null,
    fecha_nac date not null,
    calle varchar(45) not null,
    numero varchar(45) not null default 'S/N',
    colonia varchar(45) not null,
    cod_postal char(5) not null,
    telefono char(10) not null
);
```
La diferencia entre `varchar` y `char` es que varchar depende del dato para saber el tamaño de espacio que ocupará. Char es fijo.

```sh
show databases;
use temp;
describe agenda;
```

#### Borrar tabla:
```sql
drop table agenda;
```

#### Tipos de datos:
`TINYINT` $-128 \to 127$
`TINYINT UNSIGNED` $0 \to 255$


#### Modificadores numéricos
`UNSIGNED`
`AUTO_INCREMENT`

#### Tipos de datos tipo texto
`CHAR(X)`
`VARCHAR(X)`
`TEXT` no hace diferencia entre mayúsculas o minúsculas
`BLOB` si distingue entre mayúsculas

#### Modificadores de datos tipo texto
`TINYTEXT` 
`TINYBLOB`
`MEDIUMTEXT` 
`MEDIUMBLOB`
`LONGTEXT` 
`LONGBLOB`

`TEXT` y `BLOB` se usan para cadenas de texto muy extensas.

#### Tipos de datos tipo fecha
`DATE` año mes y día
`DATETIME`
`TIMESTAMP`
`TIME`
`YEAR`


#### ENUM
Podemos definir que tipo de valores puede recibir los datos de un campo que se indique como enum.

#### DEFAULT
Podemos asignar un valor por default para cada campo. Solamente `TEXT` y `BLOB` no pueden recibir un valor por default.

## Para modificar una tabla usamos el comando `ALTER`

`REMAME` sirve para cambiar el nombre de la tabla.

`CHANGE` sirve para cambiar un campo

`ADD` sirve para agregar un campo

`DROP` sirve para agregar un campo

```sql
alter table agenda
rename directorio;

alter table directorio
add email varchar(40) default 'empresa@ms.com' not null;

alter table directorio
change colonia colonia varchar(50) not null;

alter table directorio
drop email;

```

### Tarea
Investigar los comandos SQL para el comando 