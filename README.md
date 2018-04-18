# INF0175_2018
Repositorio grupo info175


Bitácora taller de construcción de software
integrantes: - Pricila Badilla
 - Andrés Gutiérrez
 - Guillermo Hernández
 - Miguel Nahuelpán
- Adolfo Cañoles

	
15/03/2018
Lluvia de ideas, para determinar qué aplicación crear.
La aplicación a crear será un registro para mejorar capacidades de los usuarios debido a sus preferencias o hobbies, como videojuegos, deportes, música,etc.
En esta aplicación el usuario tendrá su cuenta, el cual será valorado por otros usuarios, podrá compartir información el cual será visto por toda la comunidad.  
Problemas con dicha aplicación a crear ya que es muy extenso e ideas no claras.
nuevas ideas de aplicación, como la de administrar un restaurante y una aplicación web el cual consiste en preguntar al usuario: Después de terminar mi carrera yo voy a “    “, donde en el espacio se completa limitadamente por el usuario, y esta aplicación medirá por carrera lo que el usuario realizará después de finalizar su carrera.
Idea de aplicación para controlar qué cosas hacer  

20/03/2018

En la sesión de hoy terminamos por decidir la aplicación con la que trabajar, tras considerar las opciones presentes, decidimos trabajar en una aplicación para medir las horas de tiempo que dedicamos a nuestro estudio, a lo largo del día. La aplicación puede extender a más, por ejemplo horas de trabajo, horas de actividad física, etc., pero la enfocaremos al estudio con tal de poder darle una forma palpable.

Tipo de usuario: Usuario genérico
Cualquiera puede usar la aplicación, pero se espera que en sus inicios esta ayude a estudiantes y sus sesiones semanales de estudio.
La aplicación deberá poder permitir el ingreso de “ramos”, a los que asignarle durante el día horas a las que se les quiere dedicar tiempo, poder controlar cuántas horas de forma diaria se desea disponer para su estudio o ejercitación.
Se contempla que la aplicación funcione de forma independiente, es decir, solo el usuario que la descarga puede acceder a la misma donde almacena sus datos de ramos y horas que les dedica.


Link pizarra1

Ingresar actividad. 
Asignar horas a la semana para cada tarea ingresada.
Modificar la cantidad de horas a la semana.
Ingresar cuántas horas de las programadas se dedicó a la actividad.
Revisar registro de cumplimiento semanal.
Dar de baja o como concluida la tarea.







28/03/2018


Nos reunimos a las 10 AM para organizar la forma en la que presentaremos el día 29 de marzo, aclaramos algunos casos de uso y especificaciones de la aplicación, también realizamos una presentación visual(.ppt) en base a lo establecido en la sesión anterior, donde cada integrante ya tiene designado su rol:
se asignó a Andrés la presentación general del proyecto.
Pricila y Miguel sobre los casos de uso.
Guillermo explicará la interfaz pensada en la aplicación.
 
03/04/2018

Se empieza a reorganizar la información disponible:

1. Nuestro proyecto dispone de un actor, un usuario genérico.
2. Los casos de uso los agrupamos de esta forma:[- Caso de uso:] [(*) evento.]

Ingresar actividad:
            (*) ingresar nombre de la actividad.
            (*) asignar horas semanales.
Modificar actividad:
            (*) añadir horas cumplidas. 
            (*) modificar cantidad de horas. semanales
            (*) eliminar actividad.
Ver registro de cumplimiento:
            (*) registro de la semana.
            (*) registro acumulado hasta la fecha.

Link pizarra2


Código
C1
Nombre
Ingresar actividad.
Descripción
El usuario ingresa la primera actividad que desea realizar para que se genere la lista, y el tiempo semanal que dedicará a ella.
Actores
Usuario
Curso Normal
Alternativas
1. El usuario ingresa el nombre de la actividad que desea realizar.

2. El usuario ingresa una cantidad de horas que dedicará a esa actividad.



1.1  Validar nombre (este punto todavía está en discusión) *

2.1 validar hora (este punto todavía está en discusión) *








Código
C2
Nombre
Ingresar otra actividad.
Descripción
El usuario ingresa la actividad que desea realizar, y el tiempo semanal que dedicará a ella
Actores
Usuario
Curso Normal
Alternativas
1. El usuario ingresa el nombre de la actividad que desea realizar.
2. El usuario ingresa una cantidad de horas que dedicará a esa actividad.



1.1  Validar nombre (este punto todavía está en discusión) *

2.1 validar hora (este punto todavía está en discusión) *




Código
C3
Nombre
Modificar actividad
Descripción
El usuario podrá editar los datos de su actividad, según desee.
Actores
Usuario
Curso Normal
Alternativas
1. El usuario abre la opción editar (símbolo tuerca), de la actividad deseada ya creada.
2. El usuario cambiara el nombre y/o las horas que asignó inicialmente, según desee.





















Código
C4
Nombre
Eliminar actividad
Descripción
El usuario elimina la actividad de la lista de actividades disponibles
Actores
Usuario
Curso Normal
Alternativas
1. El usuario selecciona la opción de eliminar.
2. Se le pregunta al usuario que confirme que desea eliminar tal actividad, a lo que se podrá negar, o proceder.












Código
C5
Nombre
Ver actividad 
Descripción
Aquí el usuario podrá ingresar a la actividad, y agregar las horas que ha dedicado a ella, también se mostrará la efectividad total y semanal que lleva (incluye gráficos).
Actores
Usuario
Curso Normal
Alternativas
1. El usuario hace click en el nombre de la actividad en la lista de actividades creadas.
2. Se despliega el progreso en la actividad dado el momento de la semana en que se vea, como el progreso general desde que fué creada la actividad.




















Código
C6
Nombre
Añadir horas
Descripción
El usuario añade horas de progreso a la actividad deseada.
Actores
Usuario
Curso Normal
Alternativas
1. El usuario clickea el recuadro de “Añadir progreso”.
2. En el recuadro que aparece en la nueva ventana, escribe el número de horas que desea añadir.


2.1 Si se ingresa un valor no correspondiente (texto o valores no enteros positivos), se solicita que vuelva a ingresar.












05/04/2018

Se integra formalmente Adolfo Cañoles al grupo. Se ha decidido que la aplicación será de escritorio, programada con python, usando la librería tkinter. Se estudió material dispuesto en internet:

Páginas investigadas:
http://gmendezm.blogspot.cl/2012/12/tutorial-tkinter-python-gui.html
https://recursospython.com/guias-y-manuales/posicionar-elementos-en-tkinter/
http://python-para-impacientes.blogspot.cl/p/tutorial-de-tkinter.html
Documentación Tkinter

Se nos da a conocer el formato de presentaciones a partir de las próximas clases, vía slack.
El profesor nos habló sobre aspectos del proyecto, aclarar los casos de uso y nos deja agendado nuestra siguiente presentación el 19 de Abril.
Establecimos como grupo utilizar python, especificamente la version 3.6.5.
Debemos empezar a estimar cuánto tiempo nos tomará en hacer algún aspecto del programa.

-Tarea(crear repositorio en github para el grupo)

Se actualizaron las tablas presentes más arriba, añadiendo nuevos casos de uso, basados en la división de algunos previos.

	Se tomaron estas tablas para darle forma al informe solicitado en clases sobre los casos de uso, modificandolas un poco. Las mismas se estima que puedan cambiar a futuro, cosa que se registrara en el mismo informe.

18/04/2018

Se creó organización + repositorio para el proyecto en github, invitando a cada uno de los miembros del grupo y al profesor. (jueves 12 de Abril)
Luego de la clase práctica de git, cada integrante clonó el repositorio en sus computadores.

