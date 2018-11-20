### Borrar Alumno
**ID:** 004   
**Breve descripción:** El profesor borra un usuario del sistema.

**Actor principal:** Profesor   
**Actor secundario:** Alumno

**Precondiciones:**

1. El alumno debe existir en el sistema.
2. El profesor debe introducir el DNI o el Apellido.

**Flujo principal:**

1. El caso de uso empieza cuando el profesor desea borrar un alumno.   
2. El profesor introduce el DNI o el Apellido del alumno que desea borrar.   
3. El sistema recoge los datos del alumno.   
4. El sistema borra el alumno.   

**Postcondiciones:**

* El sistema muestra el alumno por pantalla.

**Flujo alternativo:**

2.a. Si no existe el alumno, el sistema muestra un mensaje de error.
2.b. Si existen dos o más alumnos con el mismo apellido, el sistema muestra una lista de esos alumnos y pregunta cual de ellos se quiere borrar.
