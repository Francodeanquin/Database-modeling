# Maratones

## Listado de Entidades
 
### Carreras **(ED)** entidad datos

- Id_carrera **(PK)**
- nombre
- tipo_carrera **(FK)**
- fecha
- tiempo        
- mejor_tiempo
- altitud
- lugar
- pais  **(FK)**
- foto

### Tipos_carreras  **(EC)** entidad catalogo

- tipo_carrera_id **(PK)**
- descripcion
- distancia

### Paises **(EC)** 

- pais_id **(PK)**
- nombre


## Relaciones

1. Una **carrera** _pertenece_ a un **tipo de carrera**. (_1 a 1_)

2. Una **carrera** se _corre_ en un **pais**.(_1 a 1_)


### Modelo Relacional de la Bd
![Modelo Relacional de la Bd] (./CarrerasModeloRelacionalBd.drawio.png)

## Reglas de negocio

### carreras

1. Crear el registro de una carrera
1. Leer el registro de una(S) carrera(s) dada ua condicion en particular.
1. Leer todos los registros de la entidad carreras
1. Actualizar los datos de una carrera
1. Eliminar los datos de una carrera dada una condicion en particular   

### tipos_carreras

1. Crear el registro de un tipo carrera
1. Leer el registro de un0(S) tipo(s) de carrera(s) dada ua condicion en particular.
1. Leer todos los registros de la entidad tipos carreras
1. Actualizar los datos de un tipo de carrera dada una condicion en particular
1. Eliminar los datos de un tipo de carrera dada una condicion en particular   

### paises

1. Crear el registro de un pais
1. Leer el registro de un pais dada una condicion en particular.
1. Leer todos los registros de la entidad paises
1. Actualizar los datos de un pais dada una condicion en particular
1. Eliminar los datos de un pais dada una condicion en particular   