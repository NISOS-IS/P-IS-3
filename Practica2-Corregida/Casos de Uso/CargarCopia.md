
### Cargar copia de seguridad  
**ID:** 008  
**Breve descripcion:** Recuperar datos de todos los alumnos.  
  
  **Actor principal:** Profesor.  
  **Actor secundario:** Alumno.
    
  **Precondiciones:**
1. la copia de seguridad debe de existir.  

**Flujo principal:**  
1. El caso de uso empieza cuando el profesor necesita cargar la copia de seguridad.
2. El sistema carga la copia de seguridad.


**Postcondiciones:**
- El sistema muestra un mensaje satisfactorio.

**Flujos alternativos:**  

2.a. En caso de no existir la copia de seguridad, mostrará un mensaje de error.  
2.b. En caso de no haber realizado la carga correctamente muestra un mensaje de error.
