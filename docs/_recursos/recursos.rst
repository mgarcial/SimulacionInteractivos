Recursos. Solo para los más curiosos
=======================================

Generación procedural:
---------------------------

* Sebastian Lague `Procedural Terrain Generation <https://youtube.com/playlist?list=PLFt_AvWsXl0eBW2EiBtl_sxmDtSgZBxB3>`__.
* Catlike Coding `Noise Derivatives, going with the flow <https://catlikecoding.com/unity/tutorials/noise-derivatives/>`__.
* t3ssel8r `Giving Personality to Procedural Animations using Math <https://youtu.be/KPoeNZZ6H4s>`__.
* Codeer `Introduction To My Weird Shooter Game - Devlog 0 <https://youtu.be/NoJXn-Fh6CU>`__.
* Codeer `Unity procedural animation tutorial (10 steps) <https://youtu.be/e6Gjhr1IP6w>`__.
* Unity `Creating a boss with procedural animation | Prototype Series <https://youtube.com/playlist?list=PLX2vGYjWbI0SwlTX_RLSD0JmzUeS0f1OK>`__.
* `GENERATIVE ART 101 <https://derivative.ca/community-post/generative-art-101-surprising-connection-between-math-art-and-nature/62742>`__.
* `Generative art <https://en.wikipedia.org/wiki/Generative_art>`__.
* `Algorithmic art <https://en.wikipedia.org/wiki/Algorithmic_art>`__.
* `Artificial intelligence art <https://en.wikipedia.org/wiki/Artificial_intelligence_art>`__.
* `Generative Art <https://cognitiveexperience.design/generative-art/>`__.


Artistas
---------

* `Casey Reas <https://reas.com/>`__.
* `feralfile <https://feralfile.com/about>`__.
* `Tony DeRose <https://youtu.be/_IZMVMf4NQ0>`__ y `este <https://youtu.be/mX0NB9IyYpU>`__.

Libros
--------

* `Basic Math for Game Development with Unity 3D <https://link.springer.com/book/10.1007/978-1-4842-5443-1#toc>`__.
* `Computational Geometry: Algorithms and Applications <https://www.amazon.com/Computational-Geometry-Applications-Mark-Berg/dp/3540779736/>`__.

Math
------

* `Linear Algebra for Games <https://www.youtube.com/watch?v=JHXUU5aqIcg>`__.
* `Essential Mathematics For Aspiring Game Developers <https://www.youtube.com/watch?v=DPfxjQ6sqrc>`__.
* `Math For Video Games: The Fastest Way To Get Smarter At Math <https://www.udemy.com/course/math-for-games/>`__.
* `Introduction to Unity.Mathematics - Unite Copenhagen <https://www.youtube.com/watch?v=u9DzbBHNwtc>`__.

Sitios 
--------

* `Use math to solve problems in Unity with C# <https://www.habrador.com/tutorials/math/>`__.
* `A community maintained Python library for creating mathematical animations <https://www.manim.community/>`__.

Videos
--------

* `Differential Equations and Dynamical Systems: Overview <https://youtu.be/9fQkLQZe3u8>`__.
* 3Blue1Brown `Differential equations, a tourist's guide <https://youtu.be/p_di4Zn4wz4>`__.
* `Solar System Simulation [Unity 3D Tutorial] <https://youtu.be/2fGL1QWMdqc>`__.
* `How to Set Up Dynamic Water Physics and Boat Movement in Unity | Ship Buoyancy Tutorial <https://youtu.be/eL_zHQEju8s>`__.
* `Craig Taylor—Outlier 2021—3d Geo Data Viz: From Insight to Data Art <https://youtu.be/wxmqG_jxJiw>`__.

Ejemplos
------------

TDAxis
*******************

Crea y transforma imágenes y sonidos con los movimientos de tu cuerpo 
`aquí <https://tdaxis.github.io/>`__.

Hydraulic Erosion
*******************

`Aquí <https://youtu.be/eaXk97ujbPQ>`__ está el ejemplo.

Atractor de Lorentz
**********************

La siguiente figura (tomada de `aquí <http://paulbourke.net/fractals/lorenz/>`__) 
corresponde a un atractor de Lorenz que es un conjunto de soluciones caóticas 
de un sistema de Lorenz.

.. figure:: ../_static/lorenzFigure.png
   :alt: Atractor de Lorenz
   :class: with-shadow
   :align: center
   :width: 100%

   Atractor de Lorenz

|

Primero quiero que veas `este <https://youtu.be/uOHkeH2VaE0>`__ video.

Ahora escucha `el tema <https://youtu.be/7zEMFt4I8k0>`__ con una animación construida 
en Unity utilizando un `atractor de Lorenz <https://en.wikipedia.org/wiki/Lorenz_system>`__.

Te dejo una parte del código para que veas que no están compleja la cosa.

.. code-block:: csharp

    void Update()
    {

        AudioListener.GetSpectrumData(spectrum, channelSelect, FFTWindow.Hanning);
        channelAvg = spectrum.Average();

        // cycle color over time
        sColor.H = hue;
        eColor.H= hue;
        line.startColor = sColor.ToColor();
        line.endColor = eColor.ToColor();
        line.startWidth = lineWidth * channelAvg * 1000;
        line.endWidth = lineWidth * channelAvg * 1000;
        hue += Time.deltaTime * oneOverColorCycleTime;
        //cycling the hue over time
        hue = hue % 1;

        float x0, y0, z0, x1, y1, z1;
        x0 = startX;
        y0 = 0;
        z0 = 0;
        float sigmaMod = sigma * channelAvg * 1000;

        for (int i = 0; i < iterations; i++)
        {
            x1 = x0 + h * sigmaMod * (y0 - x0);
            y1 = y0 + h * (x0 * (rho - z0) - y0);
            z1 = z0 + h * (x0 * y0 - beta * z0);
            x0 = x1;
            y0 = y1;
            z0 = z1;
            line.SetPosition(i, transform.position + new Vector3(x0, y0, z0));
        }
    }

