Unidad 4. Oscilaciones
=======================================

..
  Evaluación
  -----------

  Para esta evaluación te voy a proponer dos posibles proyectos. Tu elijes cuál te 
  gusta más. De todas maneras ten presente que para el proyecto que usa `fmod <https://fmod.com/>`__ 
  toca que uses tu computador porque la herramienta no está instalada en la UPB.

  Proyecto 1
  *************

  Vas a continuar enriqueciendo el proyecto del ecosistema. A medida que avances con esta simulación 
  las historias de tu ecosistema de criaturas se harán más ricas. No olvides que tu aplicación interactiva 
  en Ingeniería en Diseño de Entretenimiento Digital se queda corta si deja de contar una historia, si no 
  hay narrativa.

  Objetivo del proyecto
  ^^^^^^^^^^^^^^^^^^^^^^^^

  Crear una simulación interactiva de un ecosistema donde diferentes especies interactúan 
  y se comportan utilizando conceptos de oscilaciones, movimiento armónico simple, 
  péndulos y fuerzas de resortes. Explora cómo estas interacciones afectan el comportamiento y 
  la dinámica del ecosistema.

  Características de la simulación
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  * Creación del ecosistema: crearás un ecosistema virtual con diferentes especies, como presas, 
    depredadores y plantas. Cada especie estará representada por objetos que se comporten como 
    péndulos y fuerzas de resortes.
  * Interacción entre especies: implementarás reglas y comportamientos para que las especies 
    interactúen entre sí. Por ejemplo, los depredadores pueden ``apuntar`` a las presas y las 
    presas pueden evadir a los depredadores. Además, las especies pueden interactuar con las 
    plantas para obtener energía y nutrición.
  * Movimiento armónico simple: las especies se moverán en patrones de movimiento armónico simple. 
    Por ejemplo, las presas pueden oscilar mientras se desplazan en línea recta, y los 
    depredadores pueden realizar movimientos oscilatorios mientras persiguen a sus presas.
  * Simulación de ondas: implementarás simulaciones de ondas en el ecosistema. 
    Por ejemplo, puedes agregar un lago o un cuerpo de agua donde las ondas se propaguen y 
    afecten el comportamiento de las especies que interactúan con el agua.
  * Fuerzas de resortes: las interacciones entre las especies se basarán en fuerzas de resortes 
    simuladas. Por ejemplo, los depredadores experimentarán una fuerza de resorte al acercarse a 
    las presas, y las especies pueden experimentar fuerzas de repulsión o atracción 
    entre sí.
  * Movimiento angular: las especies pueden tener movimientos angulares que afecten su comportamiento. 
    Por ejemplo, algunas especies pueden girar para enfrentar la dirección de movimiento o 
    apuntar hacia sus objetivos.
  * Visualización interactiva: crearás una visualización gráfica que represente las especies y su 
    comportamiento en el ecosistema. Puedes usar elementos visuales para indicar las oscilaciones, 
    el movimiento armónico, las fuerzas de resortes y la dirección de movimiento de las especies.
  * Interacción del usuario: los usuarios podrán interactuar con el ecosistema y modificar 
    parámetros como la cantidad de especies, las constantes elásticas de los resortes, 
    la frecuencia y amplitud de las oscilaciones, entre otros.

  Ideas adicionales
  ^^^^^^^^^^^^^^^^^^^^^

  1. **Creación del ecosistema:**
    
    * Puedes personalizar tu ecosistema eligiendo diferentes tipos de especies con comportamientos 
      específicos. Por ejemplo, agrega especies herbívoras, carnívoras y omnívoras con distintos 
      tamaños y velocidades.
    * Establece la densidad y distribución de las especies en el entorno para influir en la 
      competencia y la disponibilidad de recursos.

  2. **Interacción entre especies:**
    
    * Implementa un sistema de alimentación donde las especies depredadoras deben cazar y atrapar 
      a las presas para obtener alimento y mantener su energía.
    * Agrega comportamientos de reproducción para que las especies puedan aumentar su población 
      y mantener un equilibrio en tu ecosistema.

  3. **Movimiento armónico simple:**
    
    * Ajusta la frecuencia y amplitud de las oscilaciones de las especies, lo que afecta su 
      velocidad y comportamiento general.
    * Experimenta con oscilaciones de diferentes patrones, como oscilaciones amortiguadas o 
      forzadas, para simular especies con comportamientos únicos.

  4. **Simulación de ondas:**

    * Agrega eventos que generen ondas en el entorno, como terremotos, movimientos de masas de agua 
      o ráfagas de viento, para afectar el comportamiento de las especies y su ubicación en el ecosistema.
    * Ajusta la intensidad y frecuencia de las ondas para ver cómo afectan a las especies y 
      cómo se propagan por todo tu ecosistema.

  5. **Fuerzas de resortes:**
    
    * Incorpora objetos o trampas con fuerzas de resorte que interactúen con las especies, como 
      redes de pesca o campos magnéticos, para afectar su movimiento y comportamiento.
    * Experimenta con resortes de diferentes constantes elásticas para simular diferentes 
      niveles de rigidez en el entorno y observa cómo afectan la movilidad de las especies.

  6. **Movimiento angular:**
    
    * Ajusta el ángulo de dirección de movimiento de las especies para que apunten hacia 
      fuentes de alimento o eviten áreas peligrosas.
    * Implementa comportamientos de orientación, donde las especies busquen seguir una 
      dirección específica, como la posición del sol o una fuente de calor.

  7. **Visualización interactiva:**
    
    * Controla la cámara para moverte libremente por el ecosistema y observar las interacciones 
      entre las especies desde diferentes perspectivas.
    * Agrega efectos visuales para representar los cambios en la energía, la salud y las 
      interacciones entre las especies, lo que te ayudará a comprender mejor los cambios en 
      tu ecosistema.

  8. **Interacción del usuario:**
    
    * Interactúa directamente con las especies utilizando el mouse para ``arrastrar`` o ``empujar`` a 
      las especies en diferentes direcciones.
    * Utiliza controles de teclado para ajustar los parámetros de las oscilaciones y fuerzas 
      de resortes en tiempo real mientras tu simulación está en marcha.
    * Explora la posibilidad de utilizar el audio como mecanismo de entrada para influir en 
      la simulación mediante comandos de voz que afecten las oscilaciones o generen eventos 
      específicos en tu ecosistema.

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
  
