
Concatenar las pegas una al lados de otras, pero con la informacion como venga directamente.

- new_dataset = pd.concat([df, df1], axis=1)

Con el merge, aunque esten desordenadas, las coloca como mejor le vienen mirando si hay algun id o columna en comun. 

- df_total = pd.merge(nombre tabla 1, nombre tabla 2, on="id que quieres coger", how="left")

Con el how = left no perdemos nada de informacion al pegar unas columnas al lado de otras. 

Sino ponemos nada, el how = inner por defecto, por lo que perderiamos informacion. 
