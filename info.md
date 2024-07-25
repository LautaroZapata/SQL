# SQL

*Informacion y notaciones de SQL*

## Modelo ER (CHEN)

### Entidad

Es una representación de algo por ejemplo una persona; la entidad de una persona representa lo que seria una persona pero hablando de forma abstracta.

En una tienda online la base de datos podría tener diferentes entidades como:

- Clientes
- Productos
- Órdenes de compra
- Proveedores

La nomenclatura que utilizamos es la **NOTACIÓN DE CHEN**.

Con esta nomenclatura podemos representar **ENTIDADES** y sus **RELACIONES**.

Utilizamos un **CUADRADO** para encerrar una **ENTIDAD**.

Una **ENTIDAD** es una entidad por sus propiedades y atributos.

Ejemplo:

**CASA**
 - Ventanas
 - Puertas
 - Direccion
 - Ubicacion
 - Etc

Estas propiedades se encierran con un **OVALO**.


![](ovalos.png)

---

### Atributos COMUNES

Dentro de los atributos comunes tenemos dos tipos:

### Atributos SIMPLES
 - Datos únicos (Ejemplo PRECIO DE CASA).



### Atributos COMPUESTOS
 - Ambientes (Porque se componen de otras cosas como tamaño, tipo, etc)

Su forma de representación es sacando una linea dando a entender que estan compuestos por otras propiedades:

![](compuestos.png)

---

### Atributos MULTIVALOR

Por ejemplo los **AMBIENTES** tienen mas de un valor, ventanas, puertas, etc.

Para su representación se les hace un **DOBLE OVALO**

![](multivalor.png)

---

### Atributos DERIVADOS

Se pueden obtener con cualquier otra información.

Por ejemplo podemos obtener la **ANTIGÜEDAD** de una casa por su **FECHA DE CONSTRUCCION**.

Lo obtenemos a partir de otro atributo.

Con la **UBICACION** nos pasaría lo mismo ya que la podemos obtener de la **DIRECCION** de la casa.

Los atributos derivados los representamos con un ovalo con su borde punteado.

![](derivados.png)

---

### KEY

Es un valor único como si fuera una Cédula de Identidad. Por ejemplo dos gemelos son iguales pero se diferencian por su Cédula de Identidad.

Lo representamos también con un óvalo pero va subrayado.

![](key.png)

---


## LENGUAJE

Para crear una BASE DE DATOS utilizamos **CREATE DATABASE "name"**, la alternativa facil en DB BROWSER es crearla desde la opcion *NEW DATABASE*



### TABLA

Es una estructura de datos que se organiza en filas y columnas.

- Nombre (Clientes,Personas,Productos,etc)
- Campo (Nombre de la columna vertical) FIELD
- Registro (Es la fila horizontal) RECORD
- Valor de Campo (Es el valor de cada celda) FIELD VALUE

Para hacerlo de forma manual seria **CREATE TABLE "name"**

---

### Valor de Campo

Los valores de campo tienen su tipo que puede ser INTEGER, TEXT, BLOB, REAL, NUMERIC.

Cada valor puede tener un DEFAULT y se repetira el valor siempre. Por ejemplo cuando no ingreso el valor por defecto se pondra el que establezca en DEFAULT.


---

*Con este codigo creamos la base de datos "users" con los campos de nombre, apellido y edad*

```sql
CREATE TABLE "users" (
	"nombre"	TEXT,
	"apellido"	TEXT,
	"edad"	INTEGER
);

```

En el apartado de EXECUTE SQL podemos agregar las consultas para nuestra base de datos.

---

### SELECT

Seleccionamos algo de la base de datos con este codigo.

Por ejemplo con el asterisco (*) podemos seleccionar todo.

Seguido de la propiedad necesitamos decir desde donde lo quiero seleccionar (FROM) y luego le decimos desde que campo.

Si queremos **SELECCIONAR TODOS LOS USUARIOS**

La consulta se veria asi:

```sql
SELECT * FROM users
```
---

### INSERT

Para insertar datos en nuestra database necesitamos hacerlo con **INSERT INTO "nombre de tabla (nombre,apellido,edad)"**.

Dentro del parentesis luego del nombre de la tabla ingresamos los campos que queremos insertar.

*Basicamente lo que decimos en la consulta es que en la tabla users queremos insertar los campos de nombre, apellido y edad.*

Esto va acompañado de los valores.

**VALUES ('Lautaro','Zapata',23)**

```sql
INSERT INTO users (nombre,apellido,edad)
VALUES ('Lautaro','Zapata',23)
```


Si queremos hacer un insert con varios valores podemos concatenarlos con coma.

```sql
INSERT INTO users (nombre,apellido,edad)
VALUES ('Lautaro','Zapata',23),
        ('Roman','Caceres',23),
        ('Santino','Zapata',11)
```

---


**Ejemplos si queremos seleccionar uno, dos o tres campos de la base de datos y esta nos devuelve una tabla nueva para cada caso**

*Seleccionamos un campo*

```sql
SELECT nombre FROM users
```
*Seleccionamos dos campos*
```sql
SELECT nombre,apellido FROM users
```

*Seleccionamos tres campos*

```sql
SELECT nombre,apellido,edad FROM users
```
---

### IDENTIFICADORES








