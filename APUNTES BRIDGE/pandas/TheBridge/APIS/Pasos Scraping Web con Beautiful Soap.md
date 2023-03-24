
Estos son los pasos generales cuando abordamos este tipo de proyectos:

1. **Identificar los elementos de la página de los que extraer la información**: Las páginas web son documentos estructurados formados por una jerarquía de elementos. El primer paso para extraer información es identificar correctamente el elemento o elementos que contienen la información deseada. Para ello, lo más fácil es abrir la página en un navegador e inspeccionar el elemento. Esto se consigue haciendo clic con el botón derecho sobre el elemento en cuestión y pulsando sobre la opción Inspeccionar o Inspeccionar elemento (depende del navegador). Quédate con toda la información disponible asociada al elemento (como la etiqueta, o los atributos id y/o class) ya que, posteriormente, te hará falta para utilizarla en Beautiful Soup.

2. **Descargar el contenido de la página**: Para ello, utiliza la librería `requests`. El contenido de la respuesta, el que contiene la página en HTML, será el que pasemos posteriormente a `Beautiful Soup` para generar el árbol de elementos y poder hacer consultas al mismo.

3. **Crear la «sopa»**: El contenido de la página obtenido en el paso anterior será el que utilicemos para crear la «sopa», esto es, **el árbol de objetos Python que representan al documento HTML**. Para ello, hay que crear un objeto de tipo `BeautifulSoup`, al cuál se le pasa el texto en formato HTML y el identificador del parser a utilizar:

        import requests

        from bs4 import BeautifulSoup

        r = requests.get('http://unapagina.xyz')

        soup = BeautifulSoup(r.text, 'lxml')

4. **Buscar los elementos en la «sopa» y obtener la información deseada**: El último paso es hacer una búsqueda en el árbol y obtener los objetos que contienen la información y datos que necesitamos.

Ejemplo: 

from bs4 import BeautifulSoup

  

# Suponemos que esta pagina de ejemplo la hemos descargado con una request

contenido = """

<html lang="es">

<head>

    <meta charset="UTF-8">

    <title>Página de prueba</title>

</head>

<body>

<div id="main" class="full-width">

    <h1>El título de la página</h1>

    <p>Este es el primer párrafo</p>

    <p>Este es el segundo párrafo</p>

    <div id="innerDiv">

        <div class="links">

            <a href="https://pagina1.xyz/">Enlace 1</a>

            <a href="https://pagina2.xyz/">Enlace 2</a>

        </div>

        <div class="right">

            <div class="links">

                <a href="https://pagina3.xyz/">Enlace 3</a>

                <a href="https://pagina4.xyz/">Enlace 4</a>

            </div>

        </div>

    </div>

    <div id="footer">

        <!-- El footer -->

        <p>Este párrafo está en el footer</p>

        <div class="links footer-links">

            <a href="https://pagina5.xyz/">Enlace 5</a>

        </div>

    </div>

</div>

</body>

</html>

"""

- soup = BeautifulSoup(contenido, 'lxml')
- type(soup.etiqueta)