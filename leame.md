       Control de Carros
 
 El objetivo de este ejercicio es diseñar un sistema de control de carros que permita gestionar la información relacionada con diferentes categorías de carros, los autos específicos disponibles en cada categoría, las personas que conducen los autos y las autopersonas asociadas con cada auto.

Analisi de definicion de requisistos

Gestión de Categorías de Carros:
RF1: El sistema debe permitir la creación, modificación y eliminación de categorías de carros.
RF2: Debe ser posible asignar múltiples autos a una categoría de carro.
RF3: Los usuarios autorizados deben poder ver la lista de categorías de carros disponibles.

Gestión de Autos:
RF4: El sistema debe permitir la creación, modificación y eliminación de registros de autos.
RF5: Debe ser posible asociar cada auto a una categoría de carro existente.
RF6: Los usuarios autorizados deben poder ver la lista de autos disponibles, incluyendo su estado (disponible o en uso).

Gestión de Personas y Autopersonas:
RF7: El sistema debe permitir la creación, modificación y eliminación de registros de personas.
RF8: Debe ser posible asignar múltiples autopersonas a un auto.
RF9: Los usuarios autorizados deben poder ver la lista de personas y su asociación con los autos.

Base de datos:
|Id           |Nombre              |Descripcion            |
|-------------|--------------------|-----------------------|
|id_categoria |nombre_categoria    |descripcion_categoria  |
|id_auto      |marca               |modelo                 |
|id_persona   |direccion           |telefono               |
|             |fecha               |eestado                |
|             |numero_placa        |año                    |
|             |                    |correo_electronico     |
|             |                    |kilometraje            | 

clasificacion de categoria de carros:
.se prodcede con la normalizacion
|ID_Categoria|	Nombre  |	Descripción    |Origen          |	Año	    |Tipo      
|------------|----------|----------------|----------------|-----------|----------|
|1           |	Sedán   |Automóviles de  |Japón           |	2022	  | Compacto |
|            |          |   t            |			      |           |          |
|            |          |           	 |		          |           |          |
|          	 |	        |                |                |           |          |
|2           |   SUV    |  Vehículos	 |Estados unidos  |  2023	  |SUV       |
|	         |          |                |                |           |          |
|3	         |Deportivo |	cupe         |Alemania	      |  2023  	  |Deportivo |
		


CREATE TABLE CategoriaCarro (
    ID_Categoria INT PRIMARY KEY,
    Nombre VARCHAR(50),
    Descripcion VARCHAR(255),
    Origen VARCHAR(50),
    Ano INT,
    Tipo VARCHAR(50)
);



