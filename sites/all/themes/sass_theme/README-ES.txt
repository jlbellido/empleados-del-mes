


- CAMBIAR EL NOMBRE DE CONFIGURACIÓN TEMA -

1 . Copiar y pegar sass_theme , no importa donde se colocan
   la versión copiada el tiempo que está en un directorio de temas . Por ejemplo, si
   están utilizando sites / all / temas se pueden colocar allí - por lo que terminan con :

   sites / all / themes / foobartheme

2 . Cambie el nombre del archivo de información y editar los detalles de información de archivo. Por ejemplo supongamos
   usted quiere que su tema se llama " foobartheme " , el nombre del archivo de información se
   ser " foobartheme.info " . Una vez que haya cambiado el nombre del archivo de abrirlo y cambio
   el "nombre" de foobartheme y cambiar la descripción para adaptarse a su gusto.

3 . Edite los archivos theme_settings.php y template.php - aquí estaremos reemplazando
   " sass_theme " con su nombre de los temas, en este caso " foobartheme " -
   este debe coincidir con el nombre que le dio al archivo info . La forma más fácil es simplemente
   utilizar búsqueda y reemplazo .

4 . Para obtener información adicional sobre el uso Adaptivetheme ver la información en
   adaptivetheme / at_core / _readme.txt

Cualquier problema por favor, publicarlo en un problema en la cola de emisión Adaptivethemes en Drupal.org :
http://drupal.org/project/issues/sass

Mantenedor:
* Nesta Guerrero https://drupal.org/user/370767
