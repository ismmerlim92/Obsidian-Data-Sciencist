Para ordenar utilizaremos el sort_values(). Con el ascending podemos cambiar el orden descendiente o ascendente, colocando True o False.

- df.groupby("ibu")["abv"].mean().sort_values(ascending = False)