### Guardar copiar de seguridad
**ID:** 007   
**Breve descripción:** El profesor guarda una copia de seguridad.

**Actor principal:** Profesor   
**Actor secundario:** Alumno

**Precondiciones:**

1. La base de datos debe contener información.

**Flujo principal:**

1. El caso de uso empieza cuando el profesor desea guardar una copia de seguridad de la base de datos.
2. El sistema genera un fichero y almacena en él la información de la base de datos.

**Postcondiciones:**

* El sistema muestra un mensaje de éxito por pantalla.

**Flujo alternativo:**

2.a. Si se produce un fallo, el sistema muestra un mensaje de error.
2.b. Si al guardar la copia ya existe un fichero con ese nombre, este se sobreescribe.
