- El atributo **contents**: Devuelve una lista con todos los hijos de primer nivel de un objeto.

- Atributo **descendants**: Este atributo devuelve un iterador que permite recorrer todos los hijos de un objeto. No importa el nivel de anidamiento.

Vamos con algunos ejemplos escritos en Python: 

- print(soup.div.div.prettify()) --- Para que salga bonito el arbol. 

- inner_div = soup.div.div

### etiqueta a

- hijos = inner_div.a

### contents

- hijos = inner_div.contents

- print(type(hijos))

- print("\n")

for child in hijos:

    if child.name:  # Ignoramos los saltos de línea

        print(f'{child.name}:\n {child.prettify()}')

        print("\n")

### descendants

- hijos = inner_div.descendants

- print(hijos)

- print("\n")

for child in hijos:

    if child.name:

        print(f'{child.name}:\n {child}')

        print("\n")

