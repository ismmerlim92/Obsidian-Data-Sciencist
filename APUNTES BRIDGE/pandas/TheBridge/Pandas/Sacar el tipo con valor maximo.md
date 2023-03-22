Hay dos formas, la primera es sacar el maximo y luego igualarlo a la columna para sacar el nombre del valor maximo: 

- max_ibu = df["nombre columna"].max()
- df[df["nombre columna"] == max_ibu]

De esta forma es mas directo pero peor:

- df.iloc[df["nombre columna"]].idxmin(), : ]