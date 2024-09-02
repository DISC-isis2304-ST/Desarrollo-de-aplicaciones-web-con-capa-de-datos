# Proyecto Guiado desarrollo de aplicaciones web con capa de datos

Se quiere diseñar una aplicación llamada Parranderos que centralice la información de bares en toda Colombia, de bebidas alcohólicas y no alcohólicas que se sirven en dichos bares y de los clientes que frecuentan dichos establecimientos junto con sus preferencias de bebida.
Para esto, ya se cuenta con el modelo de clases, pero es necesario diseñar la capa de datos de una aplicación funcional.
Con este fin, realizaremos diversas tareas a lo largo de este Proyecto Guiado para aprender a crear un modelo de entidad-relación, configurar una aplicación con acceso a una base de datos SQL a través de Spring.


## Modelo conceptual Parranderos
![](https://github.com/DISC-isis2304-ST/Introduccion-a-SQL/blob/ff4e42e9c76930f18648177404b9a1601e38040c/modelos/parranderos_UML.png?raw=true)

## Modelo Entidad/Relación

![](https://github.com/DISC-isis2304-ST/Desarrollo-de-aplicaciones-web-con-capa-de-datos/assets/77994638/e05f4d93-1358-4aef-b4cb-b70591ed9a0b)


## Modelo relacional
![](https://raw.githubusercontent.com/DISC-isis2304-ST/Introduccion-a-SQL/a584a09b5dd85b139fa699dd5083ff9e6f326897/modelos/e_relacion_parranderos.svg)

## Requerimientos técnicos
Requerimientos transversales del proyecto guiado:
- Java 17
- Maven 3.8.1
- Spring 
- Spring-JPA
- Spring Thymeleaf
- Base de datos Oracle

## Requerimientos funcionales
- **RF1 - Registrar bar**
Los bares tienen nombre, ciudad, presupuesto y cantidad de sedes. Esta operación registra un nuevo bar en la aplicación.

- **RF2 - Registrar bebedor**
Los bebedores tienen nombre, ciudad y presupuesto. Esta Operación registra un nuevo bebedor en la aplicación.

- **RF3 - Registrar bebida**
Las bebidas tienen un nombre, grado de alcohol y tipo. Está operación registra una nueva bebida en la aplicación.

- **RF4 - Registrar gustan**
Los bebedores gustan de las bebidas. Esta operación registra que un bebedor gusta de una bebida.

- **RF5 - Registrar sirven**
Los bares sirven bebidas en diferentes horarios. Esta operación registra que un bar sirve una bebida.

- **RF6 - Registrar frecuentan**
Los bebedores frecuentan bares en diferentes horarios y fechas. Esta operación registra que un bebedor frecuenta un bar.

- **RF7 - Modificar un bar**
Dado un bar que ya ha sido creado, esta operación modifica los atributos diferentes al ID del bar.

- **RF8 - Modificar un bebedor**
Dado un bebedor que ya ha sido creado, esta operación modifica los atributos diferentes al ID del bebedor.

- **RF9 - Modificar una bebida**
Dada una bebida que ya ha sido creada, esta operación modifica los atributos diferentes al ID de la bebida.

- **RF10 - Eliminar un bar**
Elimina un bar dado su ID.

- **RF11 - Eliminar un bebedor**
Elimina un bebedor dado su ID.

- **RF12 - Eliminar una bebida**
Elimina una bebida dado su ID.

- **RF13 - Ver la lista de bares**
Muestra la lista de todos los bares registrados en la aplicación.

- **RF14 - Ver la lista de bebedores**
Muestra la lista de todos los bebedores registrados en la aplicación.

- **RF15 - Ver la lista de bebidas**
Muestra la lista de todas las bebidas registradas en la aplicación.

- **RF16 - Información de gustan**
Muestra la cantidad de bebedores que gustan de bebidas con el mayor grado de alcohol y la cantidad de bebedores que gustan de bebidas con el menor grado de alcohol.

- **RF17 - Información de sirven**
Muestra la cantidad de bares que sirven bebidas con el mayor grado de alcohol y la cantidad de bares que sirven bebidas con el menor grado de alcohol.

- **RF18 - Información de bebidas**
Muestra la cantidad de bebidas que hay registradas, el promedio de grado de alcohol de las bebidas, el grado de alcohol de la bebida más alcohólica y el grado de alcohol de la bebida menos alcohólica.

- **RF19 - Filtrar bebedores por nombre**
Dado una cadena de caracteres, esta operación filtra los bebedores cuyo nombre contenga dicha cadena.

- **RF20 - Filtrar bares por ciudad y bebida**
Dado una ciudad y un tipo de bebida, esta operación filtra los bares de esa ciudad que sirven ese tipo de bebida.

- **RF21 - Filtrar bebidas por ciudad y grado de alcohol**
Dado una ciudad, un grado de alcohol mínimo y un grado de alcohol máximo, esta operación filtra las bebidas que se sirven en bares de esa ciudad con un grado de alcohol entre el mínimo y el máximo.

## Tareas 
- **Tarea 1:** [Presentación del equipo docente]
- **Tarea 2:** [Configuración básica de la aplicación](tareas/configuracion-basica-aplicacion.md)
- **Tarea 3:** [Construcción de las entidades del modelo](tareas/construccion-entidades-modelo.md)
- **Tarea 4:** [Implementación de las consultas CRUD](tareas/implementacion-consultas-CRUD.md)
- **Tarea 5:** [Construcción de controladores](tareas/construccion-de-controladores.md)
- **Tarea 6:** [Pruebas de Postman - Parte 1](tareas/pruebas-postman.md)
- **Tarea 7:** [Implementación de consultas avanzadas](tareas/implementacion-de-consultas-avanzadas.md)
- **Tarea 8:** [Pruebas de Postman - Parte 2](tareas/pruebas-postman-2.md)

## Tareas Opcionales
- **Tarea 9:** [Construcción de la interfaz – Parte 1](tareas/construccion-de-la-interfaz-parte1.md)
- **Tarea 10:** [Construcción de la interfaz – Parte 2](tareas/construccion-de-la-interfaz-parte2.md)
- **Tarea 11:** [Cambios a la interfaz](tareas/cambios-a-la-interfaz.md)




