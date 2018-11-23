La clase **Persona** es la base de la que tanto **Profesor** como **Alumno** heredan atributos comunes. Para el tratamiento de información se crean los métodos modificadores y observadores.

A su vez la clase **Profesor** tiene el atributo ***rol*** para definir si es *coordinador* o *ayudante*, los métodos getter y setter y los métodos registrarProfesor, login (para iniciar sesión), cargarCopia y guardarCopia (datos de los alumnos).

La clase **Alumno** tiene de atributos curso, equipo (al que pertenece) y líder (si lo fuese) con sus respectivos métodos getter y setter.

Por último, la clase **AgendaAlumnos**, que crea un ***List de Alumnos*** y contiene los métodos para buscar, insertar, borrar, modificar y mostrar los datos de un alumno o de todos los alumnos.
