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





