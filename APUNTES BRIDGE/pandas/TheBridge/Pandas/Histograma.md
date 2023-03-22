Un histograma es un **gráfico que se utiliza para representar la distribución de frecuencias de algunos puntos de datos de una variable**. Los histogramas frecuentemente clasifican los datos en varios “contenedores” o “grupos de rango” y cuentan cuántos puntos de datos pertenecen a cada uno de esos contenedores.

Se calcula mediante un grafico, en el que la x será el valor, y la y el numero de veces que aparece. Ejemplo:

![[Pasted image 20230321110435.png]]

df["nombre columnas"].values_counts() .... Seria un histograma feo

En panda sería para representarlo: 

- df["nombre columnas"].hist()