### Login Profesor
**ID:** 00.   
**Breve Descripción:** El profesor inicia sesión en el sistema.   

**Actor principal:** Profesor.   

**Precondiciones:**
1. El profesor debe estar guardado en el fichero binario.

**Flujo principal:**
1. El caso de uso comienza cuando el profesor quiere iniciar sesión en el sistema.
2. El sistema hace una búsqueda de las credenciales del profesor.
3. El sistema abre la sesión.

**Postcondiciones:**
+ Ninguna.

**Flujos alternativos:**

2.a. Si el profesor no se encuentra, es decir, no está guardado en el fichero, el sistema pregunta si se desea registrar.   
2.a. Si los datos son incorrectos se muestra un mensaje de error.  
2.b. Si los campos están vacíos muestra un mensaje de error.
