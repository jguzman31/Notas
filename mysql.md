# MySQL
¿Cómo ingresar a MySQL por consola?
```
cd c:/xampp/mysql/bin
```
```
mysql -h 127.0.0.1 -u root -p
```
|Letra          |Concepto    |Ejemplo                                        |
|---------------|------------|-----------------------------------------------|
|h              |Host        |IP Adress (Local,Sever) \| 127.0.0.1 (Default) |
|P (uppercase)  |Port MySQL  |3306 (Default)                                 |
|u              |User        |username                                       |
|p (lowercase)  |Password    |password                                       |

# Bases de datos
¿Cómo crear una base de datos?
```
create database <db_name>;
```
Visualizar las bases de datos.
```
show databases;
```
Acceder a la base de datos
```
use <db_name>;
```
# Tablas
¿Cómo crear una tabla?
- Una tabla es una estructura de datos que organiza en columnas y filas; cada columna es un campo (o atributo) y cada fila, un registro. La intersección de una columna con una fila, contiene un dato específico, un solo valor. 

- Cada registro contiene un dato por cada columna de la tabla. 

- Cada campo (columna) debe tener un nombre. El nombre del campo hace referencia a la información que almacenará. 

- Cada campo (columna) también debe definir el tipo de dato que almacenará.

```
CREATE TABLE usuarios(
  attribute_name_1 VARCHAR(30),
  attribute_name_2 INT,
  attribute_name_3 timestamp
);
```
Para visualizar que tablas estan creadas en la base de datos
```
show tables;
```
Para visualizar la estructura de una tabla
```
DESC <table_name>
```
MariaDB [db_name] desc <table_name>:
|Field     |Type        |Null |Key  |Default |Extra |
|----------|------------|-----|-----|--------|------|
|full_name |varchar(30) |NO   |     |NULL    |      |
|document  |varchar(15) |NO   |     |NULL    |      |
|phone     |varchar(14) |YES  |     |NULL    |      |

Modificar el nombre de una tabla
```
RENAME TABLE <old_table_name> TO <new_table_name>;
```

Eliminar una tabla (Directa)
```
DROP TABLE <table_name>;
```

Eliminar una tabla (Si existe)
```
DROP TABLE IF EXISTS <table_name>;
```
