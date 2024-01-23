Unidad 7. Bibliotecas de físicas
=======================================

..
  Evaluación
  -----------

  Llegaste a la etapa final del prototipo 1 para el portafolio. Este 
  prototipo lo has venido desarrollando todo el semestre (algunos). Es
  momento de darle el toque final. Tu simualación tendrá agentes autónomos.

  El término agente autónomo generalmente se refiere a una entidad que toma 
  sus propias decisiones sobre cómo actuar en su entorno sin ninguna influencia 
  de un líder o plan global. Para nosotros, ``actuar`` significará movimiento.

  Lo que harás esta unidad se basa en el siguiente trabajo:

  Steering Behaviors For Autonomous Characters by Craig Reynolds. GDC 1999 paper: 
  Steering Behaviors For Autonomous Characters. 
  Reynolds, C. W. (1999) Steering Behaviors For Autonomous Characters, in the 
  proceedings of Game Developers Conference 1999 held in San Jose, California. 
  Miller Freeman Game Group, San Francisco, California. Pages 763-782. El paper 
  lo puedes descargar 
  `aquí <https://github.com/juanferfranco/BookCodeSimCourse/files/11272755/gdc99steer.pdf>`__.

  Reynolds describe el movimiento de los vehículos idealizados (agentes autónomos 
  idealizados) como una serie de tres capas. En la simulación solo implementarás dos 
  de las capas (selección y dirección).

  1. Selección: un vehículo tiene un objetivo (u objetivos) y puede seleccionar 
    una acción (o una combinación de acciones) basada en ese objetivo. 
    El vehículo echa un vistazo a su entorno y calcula una acción basada en un 
    deseo: ``Veo a un zombi marchando hacia mí. Como no quiero que me coman el 
    cerebro, voy a huir del zombi``. El objetivo es mantener el cerebro y la 
    acción es huir.

    Ejemplos de objetivos: buscar un objetivo, evita un obstáculo, sigue un camino.

  2. Dirección (steering): una vez que se ha seleccionado una acción, el vehículo 
    tiene que calcular su siguiente movimiento. Para nosotros, el próximo paso será una 
    fuerza; más específicamente, una fuerza de dirección.

    Ejemplos: buscar, huir, sigue un camino, seguir un campo de flujo, reúnete con 
    tus vecinos.

  3. Locomoción.

  .. note:: RETO DE DISEÑO 

    ¿Qué significaría para su vehículo amar o tenerle miedo a su objetivo? 
    ¿Qué motiva al vehículo?


  ¿Te animas a escribir esta vez el README.md en inglés? La idea es que 
  tu portafolio pueda ser disfrutado por una audiencia global.

  Características de la simulación
  **********************************

  .. warning:: IMPORTANTE 

    Lee el texto guía. Allí encontrarás el soporte conceptual y EJEMPLOS 
    que te servirán de inspiración.

    Ten presente que para llegar a implementar las características 
    que te pido necesitarás familiarizarte con todo el material del 
    texto guía. Te recomiendo entonces que bajes el repositorio de código 
    del libro, experimentes con los ejemplos, los apropies y luego 
    los apliques a tu simulación.

  * Crea una simulación de flocking donde todos los parámetros 
    (peso de separación, peso de cohesión, peso de alineación, fuerza máxima, 
    velocidad máxima) cambian con el tiempo. Podrían ser controlados por el 
    ruido de Perlin o por la interacción del usuario mediante sliders.

  * Diseña una criatura con tantos comportamientos de dirección (steering) como 
    sea razonable. Piensa en maneras de variar los pesos de estos comportamientos 
    para que se puedan combinar en tiempo real. ¿Cómo se establecen los 
    pesos iniciales? ¿Qué reglas determinan cómo cambian los pesos con el tiempo?

  Recursos 
  ----------------------

  * El libro guía tiene ejemplos de cada una de las cosas 
    que te pido. Puedes consultar `aquí <https://natureofcodeunity.com/chaptersix.html>`__.
  * `Videos 38 al 44 <https://youtube.com/playlist?list=PLRqwX-V7Uu6ZV4yEcW3uDwOgGXKUUsPOM>`__ 
    del curso the nature of code 2. 