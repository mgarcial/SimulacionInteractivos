Unidad 3. Fuerzas
=======================================

Requisitos de la aplicación interactiva
--------------------------------------------

Vas a introducir en la simulación de la unidad anterior FUERZAS, es decir, ahora 
harás que en tu simulación ocurra lo siguiente:

.. warning:: LEE PRIMERO EL CAPÍTULO 2

    Pasos:

    1. Lee la unidad 2.
    2. Lee la unidad 2.
    3. Lee la unidad 2.

  (No es un error lo anterior, es que toca leer la unidad para 
  poder hacer la cosa bien.)

* Tus criaturas van a interactuar con elementos del ecosistema como COMIDA, 
  depredadores, plantas, etc.
* Simula fuerzas de ATRACCIÓN y REPULSIÓN entre tus criaturas y el mundo en el que viven.
* Vas a buscar ``3 tipos de fuerzas`` y las vas a ``MODELAR`` para 
  incorporarlas en la simulación, pero esas fuerzas deberán responder a una 
  ``NARRATIVA``, tu la defines, es tu ecosistema.

  .. warning:: TENEMOS UN NUEVO REQUISITO

      Desde ahora nos acompañará un nuevo requisito en la aplicación 
      interactiva: LA NARRATIVA. No lo olvides.
* Incluye en tu simulación interacción de las criaturas con líquidos donde 
  experimente fuerzas de resistencia.
* Incluye una extraña colonia de criaturas que se comporten según las ideas 
  de un n-Body problem.
* Debes adicionar interactividad a tu aplicación. Puede ser mediante teclado, 
  mouse, música, el micrófono, video, sensor o cualquier otro dispositivo 
  de entrada.
* Debes desarrollar tu aplicación bajo control de versión. Usa el directorio 
  correspondiente de cada unidad.

Trayecto de actividades
------------------------

* Realiza la lectura de la unidad 2 del texto guía: fuerzas.
* Realiza la lectura de la unidad 2. Si, no es un error, debes hacer 
  la lectura.
* Recuerdas de la unidad anterior cómo hacías para que la criatura 
  se moviera?

  .. code-block:: javascript

    let mover;

    function setup() {
      createCanvas(640, 240);
      mover = new Mover();
    }

    function draw() {
      background(255);
      mover.show();
      mover.update();
      mover.checkEdges();
    }

    ...
    update() {
      this.velocity.add(this.acceleration);
      this.velocity.limit(this.topSpeed);
      this.position.add(this.velocity);
    }        
  
  En la unidad anterior tu definías la aceleración mediante 
  algún algoritmo. Ahora la vas a calcular. ¿Qué tiene 
  que ver esto con las leyes de movimiento de Newton?

* Ahora supón que estás aplicando dos fuerzas a tu criatura:

  .. code-block:: javascript

    mover.applyForce(wind);
    mover.applyForce(gravity);
    ...
    applyForce(force) {
      this.acceleration = force;
    }

    ...
    this.velocity.add(this.acceleration);

  ¿Qué problema le ves a esto? ¿Por qué la fuerza 
  debe ser acumulativa?

* En el siguiente código:

  .. code-block:: javascript

    update() {
      this.velocity.add(this.acceleration);
      this.position.add(this.velocity);
      this.acceleration.mult(0);
    }

  * ¿Por qué es necesario multiplicar la aceleración por 
    cero en cada frame? 
  * ¿Por qué se multiplica por cero 
    justo al final de update()?
* ¿Cómo tener en cuenta la masa de la criatura?
* En el siguiente código:

  .. code-block:: javascript

    applyForce(force) {
      force.div(mass);
      this.acceleration.add(force);
    }

  * ¿force se está pasando por VALOR o por REFERENCIA?
* Cuando se modela una fuerza ¿Qué pasos hay que seguir para 
  poder incorporar dicha fuerza a la simulación?
* En el siguiente código:

  .. code-block:: javascript

    let friction = this.velocity.copy();
    let friction = this.velocity;

  * ¿Cuál es la diferencia entre las 
    dos líneas?
  * ¿Qué podría salir mal con ``let friction = this.velocity;``
  * De nuevo, toca repasar. ¿Cuál es la diferencia entre 
    copiar por VALOR y por REFERENCIA?
  * En el ejemplo cuándo es por VALOR y cuándo por REFERENCIA.


* Trabaja en tu aplicación interactiva.

Recursos 
----------------------

* `Capítulo 2 <https://natureofcode.com/forces/>`__ del texto guía.
* `Videos 17 al 22 <https://youtube.com/playlist?list=PLRqwX-V7Uu6ZV4yEcW3uDwOgGXKUUsPOM>`__ 
  del curso the nature of code 2.
