# ¿Cómo ingresar a MySQL por consola?
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

# ¿Cómo crear una base de datos?
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

# ¿Cómo crear una tabla?
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

