Hay varias formas de eliminar una columna: 

df = df.drop(columns = ["Nombre de columna"])

df = df.drop(['Nombre de columna'], axis=1)

del df['Nombre de columna']