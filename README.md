# Clasificar y subir elementos a Open Street Map

SUBIDOsM, es una aplicación basada en una bifurcación de Deriviste, que es un editor de prueba de concepto de OpenStreetMap para agregar PDI directamente desde imágenes a nivel de calle (Mapillary). Ok, no es realmente un editor ya que no puedes editar nada, solo crear.

Deriviste está escrito en JavaScript en gran parte prehistórico y tiene licencia WTFPL sin garantía. Los parches son bien recibidos. Por favor envíelos.

Orígenes de Deriviste

En octubre de 2018, Richard Fairhurst introdujo una nueva herramienta OpenStreetMap llamada Deriviste. Esta herramienta presentó al usuario una forma de crear directamente datos OSM a partir de imágenes de usuario en Mapillary, incluso haciendo clic directamente en la imagen. Gracias a una característica experimental en la biblioteca MapillaryJS de código abierto, Deriviste significa que un clic en la imagen Mapillary se tradujo a un punto en el mapa. Richard tomó prestado algún código del editor de OpenStreetMap iD para permitir la búsqueda de valores predeterminados de etiquetas OSM, luego usó la autenticación de usuario simple para permitir el envío de los datos recién creados como un conjunto de cambios OSM.

el Usuario @yopaseopor, hizo una bifurcación de esta herramienta y la llamó Deriviste_traffic_signs, tiene una interfaz simple para agregar nodos a OpenStreetMap en función de lo que ve en las imágenes de nivel de calle Mapillary, tradujo el codigo a Español y Catalan, aparte de traducir todas las etiquetas para no solo introducir señales de trafico, sino tambien diferentes elementos del mobiliario urbano como contenedores y sus tipos.

Si no tuvieras Mapillary puedes actuar de igual manera, pero te obliga a una captura de datos sobre el terreno, con mapillary puedes trabajar desde casa dado que ves los objetos en las imagenes. 

Para trabajar con la utilidad sige este procedimiento:

-Haz clic en un lugar en el mapa con elementos de Mapillary. 

-Haz doble clic en un objeto o señal de tráfico en las imágenes de la calle para colocar un nodo allí.

-Utiliza el cuadro de búsqueda para encontrar el código de este país en el preajuste.

-Completa las etiquetas usando la tabla de etiquetas de la derecha (no olvide el lado clave). Elimine el código para qué dirección no es. Deriviste screenshot4.png

-Repite hasta que hayas terminado.

-Ingresa tu nombre de usuario y contraseña de OSM, y  haz clic en 'Cargar'.

Puedes ver los cambios mediante una consulta con overpass-turbo para detectar los nuevos nodos ayudandote del asistente de consultas.

Tambien puedes exportarlo a otro editor como JOSM, Vespucci, iD o Potlatch. 

Ahora puedes adjuntar a las carreteras las señales de tráfico, eliminar los duplicados y, en general, limpiar. 

Al ser una aplicación básica a veces la API Mapillary no puede encontrar las coordenadas con un clic.

El nodo seleccionado actualmente se muestra en rojo, otros en azul. Puedes arrastrar los nodos para ajustar su posición. También puedes colocarlos haciendo doble clic sobre la cartografía.

Puede ver la aplicación funcionando en vivo en https://pepeysusmapas.github.io/SUBIDOsM/index.html

