### Modificar Alumno  
**ID:** 003  
**Breve descripcion:** Modificar datos del alumno.  
  
  **Actor principal:** Profesor.  
  **Actor secundario:** Alumno.
    
  **Precondiciones:**
1. El alumno debe existir en el sistema.  

**Flujo principal:**  
1. El caso de uso empieza cuando el profesor quiere modificar los datos de un alumno.
2. El profesor busca al alumno por DNI o apellido.
3. El profesor modifica los datos del alumno.

**Postcondiciones:**
- El sistema guarda los datos del alumno.

**Flujos alternativos:**  

2.a. Si el alumno no existe por DNI, muestra un mensaje de error.  
2.b. Si el apellido de ese alumno que se desea modificar no existe, muestra un mensaje de error.  
2.c. Si existe ese apellido pero no es el alumno buscado, el sistema pregunta si se quiere insertar.  
3.b. Si intenta añadir a un alumno como lider a un equipo que ya lo tiene asignado, el sistema modifica al alumno pero no lo pone como lider.
