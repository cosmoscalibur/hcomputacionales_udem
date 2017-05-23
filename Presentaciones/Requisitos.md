## Software requerido

### Sistema Operativo Linux

Se recomienda como distribución linux para su uso, [Ubuntu](http://www.ubuntu.com/download/desktop) LTS (16.04, 14.04). Las versiones LTS aseguran mayor estabilidad y soporte extendido (5 años) a costo de paquetes que no son muy recientes, en contraste de las versiones RR que pueden tener paquetes muy nuevos pero tienen a ser inestables por pasar por cortos periodos de tiempo en la etapa de prueba.  

Si su equipo posee bajas características de hardware, puede usar derivados de Ubuntu como [Lubuntu](http://lubuntu.net/) y [Linux Mint](https://www.linuxmint.com/) que se enfocan en este tipo de equipos, y de gran utilidad si son equipos portátiles.  

Todos los requisitos de software para el desarrollo de este curso se explica su instalación en cada sesión.  

### Python

[Python](https://www.python.org/) es un lenguaje de programación multiparadigma de amplio uso en las ciencias computacionales y computación científica, pero igualmente con una amplia comunidad en disciplinas distintas a estas. Su implementación oficial/referencia es CPython, y actualmente se encuentran vigentes las versiones Python 2 (en modo de actualizaciones de seguridad) y Python 3 (en desarrollo activo). La *PSF* recomienda el uso de python 3 para los usuarios/desarrolladores nuevos, y para los antiguos mantener python 2 solo si es realmente requerido por motivos de compatibilidad.  


La mayor parte de distribuciones linux vienen por defecto con python 2. Si no es así o si requiere python 3, podrá instalarlos por diversos métodos:  

+ Repositorios oficiales de la distribución linux. Ejemplo en sistemas debian/ubuntu:  
`sudo apt -y install python3`  
+ Distribución [Anaconda](https://www.continuum.io/downloads). Si carece de internet, posee dificultades en la estabilidad de la red o un plan de consumo por contenido descargado, descargue externamente el instalador de la distribución, el cual contiene para instalación por defecto una gran cantidad de paquetes python de uso frecuente en la computación científica, con sus dependencias.  
+ Distribución [Miniconda](http://conda.pydata.org/miniconda.html). Es una versión ligera de Anaconda, el cual instala por defecto solo el gestor de paquetes `conda` y `python`. Útil para equipos con bajas características de hardware o para una rápida descarga.  

Si usa la instalación de los repositorios o manual (no recomendada esta última), necesitará el gestor de paquetes [pip](https://pip.pypa.io/en/stable/) con el fin de instalar de la manera más simple las versiones más recientes de los paquetes (algunos vienen incluidos en los repositorios del sistema operativo). Para un sistema debian/ubuntu necesitaremos permiso de administrador y ejecutamos:  

    sudo apt -y install python3-dev python3-pip

Si desea la versión de los paquetes en python 2, simplemente omita el 3 al lado de python. El paquete `dev` es requerido como dependencia de múltiples paquetes que encontraremos al instalar con `pip` que en el caso de `conda` no es requerido ya que este empaqueta todas las dependencias (esto facilita la instalación, incluso en windows). Igualmente con `pip` requerimos de la instalación de dependencias adicionales por medio del repositorio de la distribución linux o manuales.  
