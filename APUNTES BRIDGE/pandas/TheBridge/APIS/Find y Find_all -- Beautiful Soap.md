Beautiful Soup pone a nuestra disposición diferentes métodos para buscar elementos en el árbol. Sin embargo, dos de los principales son `find_all()` y `find()`.

Ambos métodos trabajan de forma similar. Básicamente, buscan entre los descendientes de un objeto de tipo `Tag` y recuperan todos aquellos que cumplan una serie de filtros.

El filtro más básico consiste en pasar el nombre de la etiqueta a buscar como primer argumento de la función (parámetro name).

Imagina que quieres recuperar todos los enlaces (etiqueta \<a\>) que hay en el texto HTML del ejemplo. Se podría hacer del siguiente modo:

- enlaces = soup.find_all('a')

for enlace in enlaces:

        print(enlace)

Además del nombre de la etiqueta, puedes especificar parámetros con nombre. Si estos no coinciden con los nombres de los parámetros de la función, serán tratados como atributos de la etiqueta entre los que filtrar.

Por ejemplo, si quisieras encontrar el bloque `div` con `id="footer"`, podrías aplicar el siguiente filtro:

- footer = soup.find_all(id='footer')

- print(footer)

### Para mostrar el contenido sin la etiqueta:

- first_name = first_card.h2.string
- entre parentisis, hay que colocar siempre  class_=""
- .strip(), quita los espacios adelante y al final

![[Pasted image 20230323111412.png]]