### Buscar Alumno
**ID:** 001   
**Breve descripción:** El profesor busca un alumno en el sistema.

**Actor principal:** Profesor   
**Actor secundario:** Alumno

**Precondiciones:**

1. El profesor debe introducir un DNI, un Apellido o un Equipo.

**Flujo principal:**

1. El caso de uso empieza cuando el profesor desea buscar un alumno.
2. El profesor introduce el DNI, el Apellido o el número de equipo que desea buscar.
3. El sistema recoje los datos del alumno.

**Postcondiciones:**

* Ninguna.

**Flujo alternativo:**

2.a. Si no existe el alumno, el sistema muestra un mensaje de error.
2.b. Si se introduce el apellido y existen varios alumnos con el mismo, el sistema recoje los datos de cada uno de los alumnos con ese apellido.
