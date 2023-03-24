
# En la web encontramos la especificación de la API que nos interesa

url = 'https://services1.arcgis.com/hcmP7kr0Cx3AcTJk/arcgis/rest/services/Estaciones_Sevici/FeatureServer/0/query?where=1%3D1&outFields=*&outSR=4326&f=json'

  
Obtenemos los datos correspondientes con request y lo guardamos en una variable requests

- data = requests.get(url)

Escribimos el json para poder pasarlo por un Beautifier (https://codebeautify.org/jsonviewer) que nos permite visualizarlo de manera sencilla

 Guardamos la respuesta en un diccionario

# Con el método .json() de la request directamente

 leemos el json como diccionario

- data_json = data.json()

- data_json.keys()

# Sacamos los datos usando bucles o listas por comprension

- print(data_json["features"]) ---- sacamos que la informacion que queremos es attributes
- rows = [x["attributes"] for x in data_json["features"]]

# Hacemos un Dataframe de esos datos que hemos obtenido y obtenemos la tabla

- import pandas as pd

- pd.DataFrame(rows)

Hay que añadir para que siga funcionando al final de la url, Ejemplo:

- api_key = "0738bc7dab44ea96aab6d5893330bf06ed224672"

#url = f"//api.jcdecaux.com/vls/v1/stations?contract={nombre_del_contrato}&apiKey={api_key}"

- url = f"https://api.jcdecaux.com/vls/v1/contracts?apiKey={api_key}"

- req_contracts= requests.get(url)

- ls_contract = req_contracts.json()

- len(ls_contract) ------------ Vemos cuando contratos hay