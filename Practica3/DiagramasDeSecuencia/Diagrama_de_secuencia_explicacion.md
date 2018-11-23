## Buscar Alumno  
#### **Caso de uso:** 001

El actor *Profesor* quiere buscar un alumno en la agenda. *Sistema* le pedirá que indique el criterio de búsqueda, que puede ser por DNI, Apellido o Equipo. Una vez elegido dicho criterio, el Sistema realizará una consulta a *Agenda* y esta devolverá la información del alumno buscado o alumnos buscados. En caso de no existir ninguno que coincida se emitirá un mensaje de error.

## **Insertar Alumno**   
#### **Caso de uso:** 002

El actor *Profesor* inserta los datos de un alumno. Primero, *Sistema* valida los campos, de los cuales algunos son obligatorios y por tanto no pueden estar vacíos. Antes de insertarlo, realiza una consulta a la *Agenda* para ver el número de alumnos que esta ya contiene. En caso de no sobrepasar el limite, se realiza una nueva consulta, comprobando si ese alumno ya existe, si no existe el *Sistema* valida el email y comprueba si el equipo al que pertenece ya tiene líder asignado, en caso de que dicho equipo ya tenga un líder, esta campo se ignora y se guarda sin marcar, en caso contrario se asigna como líder. Una vez todo correcto, *Sistema* guarda los datos en *Agenda* y muestra un mensaje de exito si todo ha ido bien. En caso contrario, muesta un mensaje error. Si al realizar la consulta, el alumno existe, muestra un mensaje de error. Lo mismo ocurre si se intenta insertar un nuevo alumno y se ha superado el limite indicado. 

## **Modificar Alumno**   
#### **Caso de uso:** 003

El actor *Profesor* busca el alumno que desea modificar. *Sistema* realiza una busqueda de dicho alumno, si existe muestra al alumno. *Profesor* modifica la información deseada. *Sistema* valida los campos, de los cuales algunos son obligatorios y por tanto no pueden estar vacíos. Antes de modificarlo, el *Sistema* valida el email y comprueba si el equipo al que pertenece ya tiene líder asignado, en caso de que dicho equipo ya tenga un líder, esta campo se ignora y se guarda sin marcar, en caso contrario se asigna como líder. Una vez todo correcto, *Sistema* guarda los datos en *Agenda* y muestra un mensaje de exito si todo ha ido bien. En caso contrario, muesta un mensaje error. Si al realizar la consulta, el alumno no existe, muestra un mensaje de error.

## **Borrar Alumno**   
#### **Caso de uso:** 004

El actor *Profesor* introduce el DNI o Apellido del alumno que desee borrar. *Sistema* realizá una consulta a *Agenda*, si se encuentra el alumno, aparecerá un mensaje por pantalla para de confirmación de borrado. En el caso de que el alumno no se encuentra en la agenda, se mostrará un mensaje de error.

## **Mostrar Lista**   
#### **Caso de uso:** 005

El actor *Profesor* solicita al Sistema mostrar una lista de todos los *Alumnos*. *Sistema* realizá una consulta a *Agenda*, si esta contiene datos, devuelve los alumnos y *Sistema* los muestra por pantalla. En caso de que la *Agenda* esté vacía, mostrará un mensaje de error.

## **Mostrar Alumno**   
#### **Caso de uso:** 006

El actor *Profesor* indica el DNI, Apellido u Equipo del alumno o alumnos que desea mostrar. El sistema realizá una consulta a *Agenda*. En caso de coincidencia de parámetro buscado, *Agenda* devuelve el alumno o los alumnos y *Sistema* los muestra por pantalla. En caso de no existir coincidencia en la busqueda, mostrará un mensaje de error. 

## **Guardar Copia**   
#### **Caso de uso:** 007

El actor *Profesor* pide guardar una copia de Seguridad de los datos guardados en *Agenda*. *Sistema* comprueba que *Agenda* no este vacía, en este caso se cargan los datos y se realiza la copia de Seguridad. Si todo va de forma correcta, muestra un mensaje satisfactorio, en caso de algún fallo, muestra un mensaje de error. Si al hacer la copia, *Agenda* esta vacía, muestra mensaje de error.

## **Cargar Copia**   
#### **Caso de uso:** 008

El actor *Profesor* requiere cargar una copia de Seguridad en *Agenda*. *Sistema* busca dicha copia, en caso de encontrarla, la carga en *Agenda* y muestra una mensaje satisfactorio. Si hay algún fallo en el proceso, muestra un mensaje de error. En caso de que no exista ningun copia de seguridad, *Sistema* muentra mensaje de error. 

## **Registrar Profesor**   
#### **Caso de uso:** 009

El actor *Profesor* quiere registrar un nuevo usuario, indicando sus datos. *Sistema* comprueba que dicho usuario no existe, en este caso realiza el registro guardando sus datos en *FicheroProfesor* Si todo va bien, muestra un mensaje satisfactorio, en caso contrario muestra un mensaje de error. Si el usuario ya existe, pregunta si desea iniciar sesión. 

## **Login**   
#### **Caso de uso:** 010

El actor *Profesor* indica sus datos para el inicio de sesión. *Sistema* confirma el usuario haciendo una consulta en *FicheroProfesor*. Si todo esta correcto, se abre la sesión de dicho usuario. Si el login va bien, muestra mensaje satisfactorio, si ocurre algún fallo, muestra mensaje de error. En caso de que el usuario no este en el fichero, pregunta si desea registrarlo.
