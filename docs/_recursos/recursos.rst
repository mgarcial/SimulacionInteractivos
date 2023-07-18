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

Ejemplos
------------
* `Hydraulic Erosion <https://youtu.be/eaXk97ujbPQ>`__.

Atractor de Lorentz
---------------------

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

