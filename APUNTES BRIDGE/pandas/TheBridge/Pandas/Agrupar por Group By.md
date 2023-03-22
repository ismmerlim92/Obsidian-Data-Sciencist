
- df.groupby("nombre de columna que queremos agurpar")["nombre de columna de valores que queremos", "nombre de columna 2 de valores que queremos"]

ejemplo y sacamos la media: 

- df.groupby("ibu")["abv"].mean()