### Registrar Profesor
**ID:** 00.   
**Breve Descripción:** El profesor se registra en el sistema.   

**Actor principal:** Profesor.   

**Precondiciones:**
1. El profesor no debe existir en el sistema.

**Flujo principal:**
1. El caso de uso comienza cuando el profesor quiere registrarse en el sistema.
2. El profesor indica sus datos.
3. El sistema hace una búsqueda del profesor.
4. El profesor queda registrado en el sistema.

**Postcondiciones:**
+ El sistema guarda en el fichero binario los datos del profesor.

**Flujos alternativos:**

2.a. Muesta un mensaje de error si los campos están vacíos o son incorrectos.
3.a. Si el profesor ya existe, el sistema pregunta si desea iniciar la sesión.   
4.b. Muestra un mensaje de error si el fichero no se ha guardado de forma correcta.
