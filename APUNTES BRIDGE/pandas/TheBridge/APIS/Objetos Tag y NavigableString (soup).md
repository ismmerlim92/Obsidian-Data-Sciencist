![[Pasted image 20230323100816.png]]Tenemos dos tipos de objetos en Beatiful Soap: 

- **Tag**: Este objeto se corresponde con una etiqueta HTML o XML. Por ejemplo, dado el objeto soup, podemos acceder al objeto (tag) que representa al título de la página usando la etiqueta title.  Para nosotros sera un diccionario
    - soup.title

Dado un objeto de tipo Tag, podemos acceder a sus atributos tratando al objeto como si fuera un diccionario. Además, se puede acceder a ese diccionario por medio del atributo attrs:

   - div_main = soup.div

   - print(div_main)

   - print("\n")

   - print("ID Attribute:")

   - print(div_main["id"])

   - print("\n")

   - print("Attributes:")

   - print(div_main.attrs)

- **NavigableString**: Un objeto de este tipo representa a la cadena de texto que hay contenida en una etiqueta. Se accede por medio de la propiedad string.

primer_parrafo = soup.p

print(primer_parrafo, type(primer_parrafo))

texto = primer_parrafo.string

print(texto, type(texto))

type(texto)