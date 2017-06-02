# Final Herramientas computacionales

1.  Los archivos notebook de soporte que realizo para los distintos puntos, debe comprimirlos en un solo archivo `zip` con el nombre dado por la cédula seguida del primer apellido y luego la extensión. Realice este punto en la última celda de código del notebook que tenga el kernel `python` y solo cuando haya dado respuesta a todos los puntos. Adjunte el comprimido.

1.  El módulo _selenium_ puede ser usado para la recuperación de información web al igual que el módulo _requests_. Sin embargo, se diferencian en que ...
    +   _Requests_ es un módulo que emula el comportamiento de un navegador teniendo la facilidad de recuperar información dinámica de las páginas mientas que _selenium_ solo recupera el contenido estático.
    +   _Selenium_ y _requests_ poseen exactamente la misma funcionalidad, solo que _selenium_ posee un mayor consumo de recursos.
    +   ___Selenium_ es un módulo que emula el comportamiento de un navegador teniendo la facilidad de recuperar información dinámica de las páginas mientras que _requests_ solo recupera el contenido estático.__  
    +   _Selenium_ no permite recuperar información web sino solo manejar los navegadores, a diferencia de _requests_ que si puede extraer información web.

1.  El módulo _beautifoul soup_ corresponde a la funcionalidad de ...
    +   __Analizador sintáctico para lenguajes de marcado web.__
    +   Analizador sintáctico para LaTeX.
    +   Una herramienta de procesamiento de texto genérica.
    +   Un emulador de navegadores web.

1.  La herramienta de GnuPlot tiene como finalidad
    +   La creación de gráficos tridimensionales de forma interactiva.
    +   La creación de gráficos bidimensionales con enfoque en la visualización web.
    +   __La creación de gráficos 2D con un lenguaje simple a partir de tablas de datos (en archivos o en memoria).__
    +   La creación de gráficos 2D con soporte de un lenguaje de programación completo para la alta personalización de la visualización de datos contenidos en archivos.

1.  Partiendo del archivo de datos `prueba_regresion.txt`, use gnuplot  para realizar la regresión de la forma $y=a + bx^2$ del conjunto de datos asumiendo $x$ como la segunda columna y $y$ la primera columna. ¿Cual es el valor de $b$ por lo menos a 4 cifras significativas?

1.  Usando `R`, determine la densidad de probabilidad (_probability density_) para una distribución normal con $\sigma=1$ (_standard deviations_) y $\bar{x}=0$ (_mean_), para $x = 3.5$. Reporte el valor con al menos 4 cifras significativas en forma decimal. Registre el soporte de la solución de este punto en un notebook con el kernel `ir` (R).  

    __R/__:	$0.0008726827$. Dado que requerimos la densidad de probabilidad, usamos la instrucción `dnorm`. Esta instrucción posee las variables asociadas a la media y la desviación estandar definidas por defecto con los mismos valores solicitados en el punto, por lo cual no se hace necesario especificarlos. Solo necesitamos indicar el valor de `x=3.5` como argumento. Así, ejecutamos en `R`: `dnorm(3.5)` o `dnorm(3.5, 0, 1)`.  

1.  Usando expresiones regulares determine la única linea del archivo `prueba_regresion.txt` que en la primera columna posee una cantidad cuya parte entera es de dos cifras y en su parte decimal la penúltima cifra es un 5 y, en la segunda columna la primera cifra de su parte decimal es un 2 y presenta el número 8 consecutivo dos veces en la misma parte decimal.

    	grep -E '^([0-9]\{2\}\\.([0-9]*)5[0-9] ([0-9]+)\\.2([0-9]*)88)
