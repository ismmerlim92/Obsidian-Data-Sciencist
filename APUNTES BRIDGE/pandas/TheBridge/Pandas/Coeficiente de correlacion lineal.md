Va desde -1 a 1 

En [estadística](https://es.wikipedia.org/wiki/Estad%C3%ADstica "Estadística"), el **coeficiente de correlación de [Pearson](https://es.wikipedia.org/wiki/Karl_Pearson)** es una medida de dependencia lineal entre dos [variables aleatorias](https://es.wikipedia.org/wiki/Variable_aleatoria "Variable aleatoria") [cuantitativas](https://es.wikipedia.org/wiki/Variable_estad%C3%ADstica#Seg%C3%BAn_la_medici%C3%B3n "Variable estadística"). A diferencia de la [covarianza](https://es.wikipedia.org/wiki/Covarianza "Covarianza"), la correlación de [Pearson](https://es.wikipedia.org/wiki/Karl_Pearson "Karl Pearson") es independiente de la escala de medida de las variables.

De manera menos formal, podemos definir el coeficiente de correlación de Pearson como un índice que puede utilizarse para medir el grado de relación de dos variables siempre y cuando ambas sean cuantitativas y continuas.

De una forma menos coloquial, la podemos definir como el número que mide el grado de intensidad y el sentido de la relación entre dos variables.

[![formula correlación](https://economipedia.com/wp-content/uploads/2015/12/formula-correlaci%C3%B3n.png)](https://economipedia.com/wp-content/uploads/2015/12/formula-correlaci%C3%B3n.png)

Siendo:

**Cov (x;y):** la [covarianza](https://economipedia.com/definiciones/covarianza.html) entre el valor «x» e «y».

**σ(x):** desviación típica de «x».

**σ(y):** desviación típica de «y».

En Panda seria las columnas a relacionar: 

- sns.regplot(x="nombre columna", y="nombre de columna", data = df)

Muestraria un grafico asi, con la recta de regresion:

![[Pasted image 20230321105714.png]]