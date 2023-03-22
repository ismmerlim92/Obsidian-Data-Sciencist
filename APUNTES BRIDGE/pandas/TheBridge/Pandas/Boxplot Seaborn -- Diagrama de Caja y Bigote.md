
Un diagrama de caja (también, diagrama de caja y bigotes o box plot) es un **método estandarizado para representar gráficamente una serie de datos numéricos a través de sus cuartiles**. De esta manera, se muestran a simple vista la mediana y los cuartiles de los datos,​ y también pueden representarse sus valores atípicos.

Hay dos formas de escribirlo en Pandas: 

- df["nombre columna"].plot(kind ="box")
- sns.boxplot(x="nombre columna", data=df)

![[Pasted image 20230321111728.png]]