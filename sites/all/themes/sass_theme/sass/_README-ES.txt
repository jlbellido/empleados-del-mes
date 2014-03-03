

Acerca de SASS y Compass
----------------------

Este directorio incluye versiones Sass de archivos CSS de AT . Todos los archivos usan el SCSS
sintaxis .

Sass es un lenguaje que es sólo CSS normal más algunas características adicionales , como
variables, reglas anidadas , matemáticas, mixins , etc Si sus hojas de estilo están escritos en
Sass, aplicaciones de ayuda puede convertir a CSS estándar , para que pueda
incluir la CSS en los caminos normales con su tema.

Para aprender más sobre Sass, visite: http://sass-lang.com

Compass es una biblioteca de ayuda para Sass . Incluye bibliotecas de mixins compartidos , una
gestor de paquetes para agregar bibliotecas adicionales de extensión , y un ejecutable que
puede convertir fácilmente archivos Sass en CSS.

Para aprender más sobre el compás , visite : http://compass-style.org



Desarrollo con SASS y Compass
--------------------------------

Para generar automáticamente las versiones de CSS del scss mientras que usted está haciendo el tema
desarrollo , necesitará decirle a compás "vigilar " el directorio descaro para que
cada vez que un archivo scss . cambia lo colocará automáticamente una CSS generado
presentar en el directorio css de tu subtema :

  brújula <ruta reloj a su directory sub-theme's

  Si usted ya está en la raíz del directorio de su sub- tema, usted puede simplemente
  Tipo : reloj brújula

Durante el uso de CSS generado con Firebug , los números de línea que informa serán
equivocada , ya que estará mostrando los números de línea del archivo CSS generado y no el
números de línea de los archivos Sass fuente. Para corregir este problema , puede instalar
los FireSass plugin en Firefox.
  https://addons.mozilla.org/en-US/firefox/addon/firesass-for-firebug/

Si no desea utilizar Ruby y la línea de comandos se puede extraer la Sassy
proyecto para Drupal : http://drupal.org/project/sassy

Mudarse a Producción 
-------------------- 

Una vez que haya terminado su desarrollo sub-tema y están dispuestos a mover su CSS 
archivos en el servidor de producción, tendrá que indicar a sass para actualizar todo tu CSS 
archivos y comprimirlos (para mejorar el rendimiento). Nota: el comando de Compass 
sólo generará CSS para archivos SCSS que han cambiado recientemente,. con el fin de 
obligarlo a regenerar todos los archivos CSS, puede utilizar el comando limpia la brújula '
para borrar todos los archivos CSS generados. 

- Eliminar todos los archivos CSS ejecutando: brújula limpia 
- Editar el archivo config.rb en el directorio de su tema y descomentar esta línea 
   la supresión de la "#" de la beginnning: 
     # = ambiente: producción 
- Regenerar todos los archivos CSS ejecutando: brújula compilar 

Y no te olvides de encender la agregación CSS de Drupal. :-)
