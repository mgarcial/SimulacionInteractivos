Unidad 4. Oscilaciones
=======================================

Evaluación
-----------

Para esta evaluación te voy a proponer dos posibles proyectos. Tu elijes cuál te 
gusta más. De todas maneras ten presente que para el proyecto que usa `fmod <https://fmod.com/>`__ 
toca que uses tu computador porque la herramienta no está instalada en la UPB.

Proyecto 1
*************

Vas a continuar enriqueciendo el proyecto del ecosistema.


Proyecto 2
*************

En este caso será un proyecto de música generativa basada en oscilaciones, péndulos y fuerzas 
de resortes utilizando FMOD.


Objetivo del proyecto
^^^^^^^^^^^^^^^^^^^^^^^^

Crear una aplicación musical generativa donde los usuarios puedan interactuar con 
oscilaciones, péndulos y fuerzas de resortes para componer y manipular música de manera 
intuitiva. Se utilizará la biblioteca FMOD para la generación y reproducción de sonido.

Características de la aplicación
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Generación de notas musicales: la aplicación generará notas musicales basadas en oscilaciones, 
  movimientos armónicos de péndulos y fuerzas de resortes. La posición y velocidad de los 
  péndulos y las deformaciones de los resortes determinarán la altura y duración de las 
  notas generadas.
* Control de parámetros: los usuarios podrán ajustar diferentes parámetros, como la longitud de 
  los péndulos, la constante elástica de los resortes, la masa de los objetos, etc., 
  para modificar el sonido resultante.
* Interacción en tiempo real: la música se generará en tiempo real mientras los usuarios 
  interactúan con los controles y los elementos de la aplicación. Cada cambio en los parámetros 
  afectará la música de inmediato.
* Instrumentos virtuales: la aplicación utilizará FMOD para ofrecer una selección de instrumentos 
  virtuales que los usuarios pueden elegir para reproducir las melodías generadas. 
  Cada instrumento estará asociado con diferentes parámetros físicos de los péndulos y 
  los resortes.
* Armonización y acordes: Se incorporarán reglas de armonía y acordes basados en la 
  interacción entre diferentes oscilaciones y fuerzas de resortes para crear progresiones 
  musicales coherentes.
* Visualización sincronizada: La aplicación incluirá una visualización gráfica que 
  represente los péndulos y las fuerzas de resortes mientras la música se reproduce, 
  lo que permitirá a los usuarios ver cómo sus interacciones afectan la generación musical.

Implementación con FMOD:
^^^^^^^^^^^^^^^^^^^^^^^^^

Para utilizar FMOD en este proyecto, deberás seguir los siguientes pasos:

* Importar FMOD en Unity: descarga e importa el paquete FMOD para Unity en tu proyecto.
* Creación de eventos de sonido: utiliza la herramienta FMOD Studio para crear eventos de 
  sonido que representen los instrumentos virtuales y sus variaciones de sonido en función de 
  los parámetros físicos de los objetos oscilantes.
* Integración con Unity: configura la integración de FMOD en Unity y establece la comunicación 
  entre los objetos oscilantes y los eventos de sonido creados en FMOD Studio.
* Mapeo de parámetros: asocia los parámetros físicos de los péndulos y fuerzas de resortes con 
  los parámetros de sonido en FMOD para que los movimientos y oscilaciones de los objetos afecten 
  la generación musical.
* Reproducción de sonido: utiliza las API de FMOD en Unity para reproducir los eventos de sonido 
  generados en FMOD Studio en función de las interacciones del usuario con los controles de la 
  aplicación.

Integración de fmod con Unity: idea general 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Paso 1: Descargar e importar FMOD en Unity
+++++++++++++++++++++++++++++++++++++++++++

* Ve al sitio web de `FMOD <https://fmod.com/>`__ y descarga el paquete FMOD para Unity que 
  corresponda a tu versión de Unity.
* Importa el paquete FMOD en tu proyecto de Unity seleccionando ``Assets`` en el menú y luego 
  ``Import Package``, ``Custom Package``. Selecciona el archivo del paquete FMOD descargado.
  
Paso 2: Configurar FMOD Studio
+++++++++++++++++++++++++++++++

* Descarga e instala FMOD Studio desde el sitio web de `FMOD <https://fmod.com/>`__. 
  FMOD Studio es una herramienta de edición de audio que te permitirá crear eventos de sonido 
  para tu proyecto de Unity.
* Abre FMOD Studio y crea un nuevo proyecto para tu aplicación musical generativa.

Paso 3: Crear eventos de sonido en FMOD Studio
++++++++++++++++++++++++++++++++++++++++++++++++

* En FMOD Studio, crea eventos de sonido que representen los instrumentos virtuales y 
  variaciones de sonido que deseas utilizar en tu aplicación. Un evento puede representar 
  un instrumento específico, como un piano o un sintetizador, y puedes definir diferentes 
  variaciones para diferentes parámetros de sonido.
* Define los parámetros de sonido en FMOD Studio que estarán vinculados a los parámetros 
  físicos de los péndulos y las fuerzas de resortes en Unity. Por ejemplo, puedes tener 
  parámetros para la frecuencia, la amplitud o la duración del sonido.

Paso 4: Configurar la integración de FMOD en Unity
++++++++++++++++++++++++++++++++++++++++++++++++++++

* En Unity, ve al menú ``Window`` y selecciona ``FMOD Studio`` para abrir el panel de configuración 
  de FMOD en Unity.
* En el panel de configuración, establece la ruta del proyecto de FMOD Studio que creaste previamente.

Paso 5: Crear scripts de interacción con FMOD en Unity
++++++++++++++++++++++++++++++++++++++++++++++++++++++++

* Crea scripts en C# en Unity para manejar la interacción entre los objetos oscilantes y los 
  eventos de sonido creados en FMOD Studio.

* En los scripts, utiliza las API de FMOD en Unity para reproducir y controlar los eventos de 
  sonido en función de las interacciones del usuario con los controles de la aplicación.

Paso 6: Mapear parámetros físicos con parámetros de sonido
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

* Asocia los parámetros físicos de los péndulos y fuerzas de resortes con los parámetros de 
  sonido en FMOD. Puedes hacer esto utilizando las funciones de FMOD en Unity para cambiar 
  los valores de los parámetros de sonido en tiempo real según los movimientos y oscilaciones 
  de los objetos.

Paso 7: Reproducción de sonido
+++++++++++++++++++++++++++++++++

* En la aplicación de Unity, cuando los usuarios interactúen con los controles y los objetos 
  oscilantes, activa los eventos de sonido correspondientes en FMOD utilizando los scripts 
  que creaste. Esto reproducirá el sonido generado en función de las interacciones del usuario 
  con los parámetros físicos de los objetos.

Trayecto de actividades
------------------------

* MIRA por favor el plazo de entrega de esta unidad. ¿Lo tienes claro?
* Planea cómo vas a invertir el tiempo basado en el plazo.
* Lo primero que harás es leer con atención la evaluación propuesta.
* Revisa con detenimiento el `capítulo 3 <https://natureofcodeunity.com/chapterthree.html>`__ del 
  texto guía.

Recursos 
----------------------

* `Capítulo 3 <https://natureofcodeunity.com/chapterthree.html>`__ del texto guía.
* `Videos 23 al 31 <https://youtube.com/playlist?list=PLRqwX-V7Uu6ZV4yEcW3uDwOgGXKUUsPOM>`__ 
  del curso the nature of code 2.
* `fmod <https://fmod.com/>`__.
* Video que muestra la idea general de fmod. 
  `FMOD Studio Tutorial. How to Create Adaptive Audio for Video Games <https://youtu.be/7A1HMOsD2eU>`__.
* Video que muestra como usar fmod con Unity. 
  `How to make an Audio System in Unity. Unity + FMOD Tutorial <https://youtu.be/rcBHIOjZDpk>`__.
 