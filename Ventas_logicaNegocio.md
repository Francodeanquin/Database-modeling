# ventas

## Listado de Entidades

### clientes **(ED)**

- cliente_id **(PK)**
- nombre
- apellidos
- telefono  **(UQ)**
- email **(UQ)**
- direccion 
- cp
- ciudad
- pais **(FK)**

### productos **(EC)**

- producto_id **(PK)**
- nombre 
- descripcion
- foto
- precio
- cantidad

### ventas

- venta_id **(PK)**
- cliente_id  **(FK)**
- fecha 
- monto

### articulos_x_venta **(EP)**
- articulo_id **(PK)**
- venta_id **(FK)**
- producto_id **(FK)**
- cantidad 

### paises **(EC)**

- pais_id **()**
- nombre
- dominio **(UQ)**


## relaciones

1. Un **cliente**  tiene **pais**(_1 a 1_)
2. un **cliente** genera **ventas**(_1 - M_)
3. una **venta** tiene **articulos** (_1 a M_)
1. un **articulo** es un **producto** (_1 a 1_)