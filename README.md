# Trabajar con los recursos offline

## JavaScript

### En la parte frontend (el cliente/usuario).

Todos los navegadores web contienen un entorno de ejecución de código JavaScript. Abriendo una página web en un navegador, esta puede hacer uso de código JavaScript que esté embebido `<script>` en ella.

### En la parte backend (el servidor web)

O en cualquier otra ocasión donde no se trabaje dentro de un navegador web. El entorno de ejecución JavaScript más popular es Node.js
https://nodejs.org/es

Aunque, haciendolo así, no se tiene acceso al contexto BOM (Browser Object Model) ni al DOM (Document Object Model). Por ejemplo, no se tiene acceso ni a `window` ni a `document`.

Pero se gana acceso a otros contextos exclusivos de Node, como el que permite acceder sin restricciones al disco del ordenador o a sus conexiones de red.

## Bootstrap

- Descargar la versión compactada y minimizada desde: https://getbootstrap.com/docs/5.3/getting-started/download/

  (El enlace "download" desde la página principal: https://getbootstrap.com/)

- Descomprimir el .zip descargado y poner el contenido de sus dos carpetas en las correspondientes carpetas 'css' y 'js' de nuestro proyecto.

- Poner el correspondiente enlace al css, en la cabecera de nuestras páginas (dentro de `<head>`):

  `<link rel="stylesheet" href="css/bootstrap.min.css">`

- Poner la correspondiente carga de código, hacia el final del cuerpo de nuestras páginas (cerca de `</body>`) :

  `<script src="js/bootstrap.min.js"></script>`

## JQuery

- Descargar la versión compactada y minimizada desde: https://jquery.com/download/

  (nota: Para descargar el archivo en lugar de visualizarlo, hacer clic-dcho sobre el enlace y guardarenlacecomo)

- Poner ese archivo en la correspondiente carpeta 'js' de nuestro proyecto.

- Poner la correspondiente carga de código, hacia el final del cuerpo de nuestras páginas (cerca de `</body>`) :

  `<script src="js/jquery-3.7.0.min.js"></script>`

nota: Los scripts que hacen uso de JQuery se han de escribir detrás de esa línea de carga de código. Usar selectores (https://learn.jquery.com/using-jquery-core/selecting-elements/) para hacer referencia a las partes de la página a las que afectan los scripts.

nota: El código ha de estar cargado antes de que aparezca ninguna referencia a `$` en la página. Si escribimos directamente algún script que use JQuery en algún punto en el cuerpo de la página, la carga de código deberia ir al principio (dentro de `<head>`).

## JQuery User Interface

- Descargar desde https://jqueryui.com/download/

- Descomprimir el .zip descargado (es una demo de funcionamiento)

- Coger los archivos .css y ponerlos en la correspondiente carpeta 'css' de nuestro proyecto.

- Coger los archivos .js y ponerlos en la correspondiente carpeta 'js' de nuestro proyecto.

- Coger la carpeta 'images' y ponerla en nuestro proyecto.

- Si ya tenemos JQuery en nuestro proyecto, no es necesario hacer nada con la carpeta 'external'

- Poner el correspondiente enlace al css, en la cabecera de nuestras páginas (dentro de `<head>`):

  `<link href="css/jquery-ui.css" rel="stylesheet" />`

- Poner la correspondiente carga de código, hacia el final del cuerpo de nuestras páginas (cerca de `</body>`) :

  `<script src="js/jquery-ui.js"></script>`

  nota: Los scripts que hacen uso de JQuery se han de escribir detrás de esa línea de carga de código. Usar selectores (https://learn.jquery.com/using-jquery-core/selecting-elements/) para hacer referencia a las partes de la página a las que afectan los scripts.
