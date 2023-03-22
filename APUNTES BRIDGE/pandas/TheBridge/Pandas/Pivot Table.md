Es para agregar los valores que nos piden en una tabla, parecida al Excel:

- table = pd.pivot_table(df, values=' nombre columna de valor que quieres', index=['nombre indice 1', 'nombre indice 2'], columns=['otra columna'], aggfunc=[np.sum, np.mean, np.median, np.max])