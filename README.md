<div align='center'>
  
  # Indice de marginación
  
</div>

## Detalles del proyecto

En este trabajo, nos enfocaremos en analizar una base de datos de la CONAPO, la cual posee por municipio y estado indicadores de el nivel de marginación de la población. Para hacer este trabajo, hicimos uso de python en libteras jupyter, utilizando librerías como pandas, numpy, matplotlip, entre otras.

### Descargar y leer el archivo

La base de datos se descargó directamente de la página de la CONAPO, este archivo se encontraba en formato .xls y contaba con 3 pestañas. Para que fuera útil y poder manejarlo en python, se guardó el archivo como formato .csv, seleccionando la  hoja del libro correspondiente ('IMM_2020' en este caso).

### Mostrar la descripción del DataFrame

Para ello, despué de leer la base de datos, se estableció el dataframe que contuviera la información de la base de datos. Una vez establecido el dataframe, se le aplica la función _'.describe()'_ para que nos diera una descripción general de las variables contenidas.

### Realizar una gráfica de porcentaje municipios por estado vs indice de marginación 

En este punto el porcentaje de municipios por estado contra el indice de marginación y después se guardá la figura resultante en formato png

### Realizar una gráfica de porcentaje población respecto a la población total

En este caso, se realizó la gráfica del porcentaje de la población con respecto a la población de cada estado. La gráfica que nos dé de resultado, será almacenada en formato jpg

### Analizar gráficas anteriores

Aquí observamos las similitudes y diferencias que poseían ambas gráficas. De forma general, se observó que la gráfica de porcentaje municipios nos daba unos índices de marginación más preocupantes, pero ya al observarlo en la gráfica de porcentaje poblacióm, se llegó a la conclusión que los municipios pequeños hacen mucho ruido en la primera gráfica y no son tan significativos.

### Graficar la relación porcentaje analfabetismo vs porcentaje población localidades menores a 5,000

En esta gráfica, se esperaba observar que hubiera una relación entre el analfabetismo de la población con comunidades que tuvieran un menor número de habitantes. Visualmente no se logró apreciar una relación entre ambas variables, por lo cuál se utilizó el coeficiente de correlación para tener algo cuantificable que nos demostrará una relación, el resultado fue de 0.45, lo que nos quiere decir que no existe ninguna correlación entre estos dos valores.

### Variable con más relación al porcentaje de analfabetismo

Para saber cual es la variable que posee una mayor correlación con el porcentaje de analfabetismo, se realizó un mapa de calor, y nos concenctramos en la fila y/o columna del porcentaje de analfabetismo, observamos como se comportaban las demás variables con respecto a ésta y se encontró que la variable sin educación básica fue quién tenía la mayor correlación, con un valor de 0.78

### Desarrollar un nuevo DataFrame

Para este punto utilizamos algunas características del dataframe original, aquellas referentes al nombre y clave de municipios y estados.

Una vez hecho eso, propuse 4 indicadores que podrían ser de ayuda analizar cuando se desee hacer una política pública. Estos indicadores elegidos fueron los que a mi parecer son influyentes a la hora de considerar hacer una obra pública, sin embargo, se deben de obtener datos de campo y hacer una análisis de estos para lograr tener una certeza de si son o no relevantes.
