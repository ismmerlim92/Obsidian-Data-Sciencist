
En [estadística](https://es.wikipedia.org/wiki/Estad%C3%ADstica "Estadística"), la **desviación típica** (también conocida como **desviación estándar** y **desvío típico** y representada de manera abreviada por la letra griega minúscula sigma **[σ](https://es.wikipedia.org/wiki/%CE%A3 "Σ")** o la letra latina [s](https://es.wikipedia.org/wiki/S "S"), así como por las siglas **SD** (de _standard deviation_, en algunos textos traducidos del inglés)) es una medida que se utiliza para cuantificar la variación o la [dispersión](https://es.wikipedia.org/wiki/Medidas_de_dispersi%C3%B3n "Medidas de dispersión") de un conjunto de datos numéricos.[1](https://es.wikipedia.org/wiki/Desviaci%C3%B3n_t%C3%ADpica#cite_note-StatNotes-1)​

Una desviación estándar baja indica que la mayor parte de los datos de una muestra tienden a estar agrupados cerca de su [media](https://es.wikipedia.org/wiki/Media_(matem%C3%A1ticas) "Media (matemáticas)") (también denominada el _valor esperado_), mientras que una desviación estándar alta indica que los datos se extienden sobre un rango de valores más amplio.

![{\displaystyle s={\sqrt {\frac {\sum _{i=1}^{N}(x_{i}-{\overline {x}})^{2}}{N-1}}}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/00eb0cde84f0a838a2de6db9f382866427aeb3bf)


Mientras mas se aleje de la media, habra mas desviacion tipica y mayor dispersion. 

Ejemplo: 

Numero: 0 y 10. Media 5, pero con mucha desviacion tipica.

Numero 5 y 5. Media 5, no tendra desviacion tipica y no tendra dispersion. 

En Panda sera: 

1 Necesitamos la media y la desviacion estandar para tener mas informacion:

- std = df["nombre columna"].std()
- mean = df["nombre columna"].mean()

print(f"La media es de {mean} y la desviacion estandar es {std})

ej:

print(f" el amargor de la cerveza estara entre {mean - std} y {mean + std})