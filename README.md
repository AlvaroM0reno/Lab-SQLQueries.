Laboratorio | Consultas SQL 5
En esta práctica de laboratorio, utilizará la base de datos de alquiler de películas de Sakila . Ya ha estado utilizando esta base de datos en un par de laboratorios, pero si necesita obtener los datos nuevamente, consulte el enlace de instalación oficial .

La base de datos está estructurada de la siguiente manera: esquema de base de datos




Instrucciones
Suelte la columna picturede staff.

Se contrata a una nueva persona para ayudar a Jon. Su nombre es TAMMY SANDERS y es cliente. Actualice la base de datos en consecuencia.

Agregue el alquiler de la película "Academy Dinosaur" de Charlotte Hunter de Mike Hillyer en la Tienda 1. Puede usar la fecha actual para la rental_datecolumna de la rentaltabla. Sugerencia : consulte las columnas de la tabla de alquiler y vea qué información necesitaría agregar allí. Puede consultar esos datos. Por ejemplo, notarás que customer_idtambién necesitas información. Para conseguirlo puedes utilizar la siguiente consulta:

select customer_id from sakila.customer
where first_name = 'CHARLOTTE' and last_name = 'HUNTER';
Utilice un método similar para obtener inventory_id, film_idy staff_id.

Elimine los usuarios no activos, pero primero cree una tabla de respaldo deleted_users para almacenar customer_id, emaily datepara los usuarios que se eliminarían. Sigue estos pasos:

Compruebe si hay usuarios no activos
Cree una tabla de respaldo de tabla como se sugiere
Insertar los usuarios no activos en la tabla de respaldo de la tabla.
Eliminar los usuarios no activos de la tabla de clientes.
