Unidad 2. Vectores
=======================================

Requisitos de la aplicación interactiva
--------------------------------------------

Vas a imaginarte una población de CRIATURAS COMPUTACIONALES en un ecosistema digital, 
interactuando unos con otros de acuerdo con varias reglas.

* Vas a diseñar al menos 3 criaturas que tengan:

  * Apariencia diferente.
  * Desarrolla un conjunto de reglas para simular el comportamiento de cada criatura. 
    Por ejemplo: una mosca nerviosa, un pez nadando, un conejo saltando, una 
    serpiente deslizándose, etc.
  * Controla el movimiento de la criatura ÚNICAMENTE manipulando la ACELERACIÓN.
  * Dale personalidad a la criatura a través de su comportamiento.
  * Asegúrate que al menos una criatura, usando vectores, implemente una caminata aleatoria 
    y un vuelo de `Lévy <https://natureofcode.com/random/>`__ (mediante una distribución 
    personalizada de números aleatorios). Por ejemplo, el siguiente código muestra un random walker 
    con una probabilidad del 1% de realizar un paso enorme. Mira el capítulo anterior para 
    repasar.

.. code-block::javascript

    let r = random(1);
    if (r < 0.01) {
      xstep = random(-100, 100);
      ystep = random(-100, 100);
    A 1% chance of taking a large step

    } else {
      xstep = random(-1, 1);
      ystep = random(-1, 1);
    }

* Debes adicionar interactividad a tu aplicación. Puede ser mediante teclado, 
  mouse, música, el micrófono, video, sensor o cualquier otro dispositivo 
  de entrada.
* Debes desarrollar tu aplicación bajo control de versión. Usa el directorio 
  correspondiente de cada unidad.

Trayecto de actividades
------------------------

* Realiza la lectura de la unidad 1 del texto guía.
* Experimenta con los conceptos y el código. Documenta las conclusiones que 
  vas descubriendo.
* Trabaja en tu aplicación interactiva.

Recursos 
----------------------

* `Capítulo 1 <https://natureofcode.com/vectors/>`__ del texto guía.
* `Videos 10 al 16 <https://youtube.com/playlist?list=PLRqwX-V7Uu6ZV4yEcW3uDwOgGXKUUsPOM>`__ 
  del curso the nature of code 2.




..
  Evaluación
  -----------

  En el `capítulo 1 <https://natureofcodeunity.com/chapterone.html>`__ del texto 
  guía se propone un proyecto al final denominado ``The Ecosystem Project``. La 
  evaluación consiste entonces en simular un ecosistema. 

  Vas a imaginarte una población de CRIATURAS COMPUTACIONALES nadando alrededor 
  de un estanque digital, interactuando unos con otros de acuerdo con varias reglas.

  * Vas a diseñar al menos 3 criaturas.
  * Desarrolla un conjunto de reglas para simular el comportamiento de cada criatura. 
    Por ejemplo: una mosca nerviosa, un pez nadando, un conejo saltando, una 
    serpiente deslizándose, etc. ¿Cuáles serían esas reglas de comportamiento para 
    las criaturas del estanque digital?
  * Controla el movimiento de la criatura únicamente manipulando la aceleración.
  * Dale personalidad a la criatura a través de su comportamiento en lugar de su diseño 
    visual.
  * Asegúrate que al menos una criatura, usando vectores, implemente una caminata aleatoria 
    y un vuelo de Lévy (mediante una distribución personalizada de números aleatorios).

  .. note:: PARA LA ENTREGA DE LA EVALUACIÓN

    No olvides incluir en la explicación cómo resolviste cada uno de los puntos anteriores. 
    Sin esta explicación no se recibirá la evaluación. ¿Vale?

  Trayecto de actividades
  ------------------------

  * MIRA por favor el plazo de entrega de esta unidad. ¿Lo tienes claro?
  * Planea cómo vas a invertir el tiempo basado en el plazo.
  * Lo primero que harás es leer con atención la evaluación propuesta.
  * Revisa con detenimiento el `capítulo 1 <https://natureofcodeunity.com/chapterone.html>`__ del 
    texto guía.
  * Responde la siguiente cuestión: Qué es motion 101 y explica la idea.
  * Ahora analiza con detenimiento la sección ``1.8 Vector Motion: Acceleration``. Explica 
    en términos geométricos cuál sería la relación entre la posición, la velocidad, la aceleración 
    y la fuerza.

  Recursos 
  ----------------------

  * `Videos 10 al 16 <https://youtube.com/playlist?list=PLRqwX-V7Uu6ZV4yEcW3uDwOgGXKUUsPOM>`__ 
    del curso the nature of code 2.
