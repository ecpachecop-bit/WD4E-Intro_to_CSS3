# Verificación de la Tarea 2

Fecha de preparación: 20 de septiembre de 2026.

## Resultado y alcance

Se comprobaron localmente la estructura requerida, las rutas de navegación,
los selectores CSS y el comportamiento del enlace de salto mediante teclado.
Estas pruebas NO son una validación oficial de WAVE ni del servicio W3C.

| Comprobación | Resultado |
|---|---|
| Páginas con una única hoja CSS, en la ruta correcta | 3 de 3. |
| IDs de destino del enlace de salto únicos y presentes | 3 de 3. |
| Primer control enfocable: enlace de salto | Correcto en los 12 escenarios de navegador. |
| Tab muestra el enlace; Enter transfiere el foco a main | Correcto en los 12 escenarios. |
| Imagen situada dentro de nav | Correcto en las tres páginas. |
| Selectores activos de li | 0; ambas reglas anteriores están comentadas. |
| Análisis sintáctico con tinycss2 | 0 errores detectados en reglas y declaraciones. |
| Declaraciones reconocidas por CSS.supports en Chromium | 145 de 145. |
| nav: display calculado | inline-block. |
| nav: proporción medida | 80% del ancho de su contenedor, con redondeo subpíxel. |
| nav img: proporción medida | 10% del contenedor interior, con redondeo subpíxel. |
| Grid | Dos columnas del 40%, imágenes al 100% de su columna. |
| Flexbox | display:flex y flex-wrap:wrap, con anchos independientes del Grid. |
| Rutas de los enlaces internos | Los destinos corresponden a los tres HTML presentes. |
| Referencias a las fotografías | Los 20 nombres únicos coinciden con el árbol de imágenes consultado del repositorio. |

Se renderizaron las tres páginas a 320, 390, 768 y 1366 píxeles de ancho
(12 escenarios). No se detectó desbordamiento horizontal en esas pruebas.

## Condiciones de la prueba de navegador

El entorno no permitió navegar al servidor local ni descargar las fotografías.
Para comprobar el CSS y el teclado, se cargó una copia de cada documento en
memoria en Chromium y se inyectó exactamente el contenido de su hoja CSS.
Solo en la prueba se sustituyeron las fotografías por imágenes de dimensiones
de referencia. Esas imágenes de prueba NO se incluyen en el ZIP ni en el HTML
entregado; las páginas finales conservan las rutas reales de las fotografías.

Por tanto, la prueba comprueba las proporciones, el espaciado, los selectores y
el foco, pero NO acredita la carga ni la apariencia final de las fotografías en
el sitio publicado. La navegación entre páginas se verificó por sus rutas y
archivos de destino, no con clics sobre una publicación en GitHub Pages.

## Contraste calculado

Se examinaron colores de texto y sus fondos opacos en estados predeterminados,
de hover y de foco de los controles examinados. La relación mínima calculada
fue aproximadamente **7,23:1**. El cálculo se hizo a partir de la luminancia
relativa; no es un resultado de WAVE ni certifica toda la accesibilidad.

## Pendiente después de subir la carpeta

1. Esperar a que GitHub Pages publique la carpeta nueva.
2. Abrir cada página y confirmar que cargan todas las fotografías.
3. Comprobar el menú y el enlace de salto sobre la publicación real.
4. Ejecutar WAVE y W3C sobre las tres URLs de la Tarea 2.
5. Corregir los errores que indiquen los validadores y volver a comprobar.

Los informes mostrados anteriormente por el usuario corresponden a la Tarea 1;
no se han reutilizado como evidencia para la Tarea 2.

## Copia conservada

No se ha enviado ninguna modificación al repositorio. El ZIP añade únicamente
la carpeta CSS-week2-HW2 cuando se sube a la raíz, sin tocar CSS-week1-HW1.
Las imágenes se comparten mediante rutas ../CSS-week1-HW1/images/.

SHA de los archivos de la Tarea 1 usados como base:

```text
index.html        2ae19cfef5cda266fee660bda25542263f148eca
neighborhood.html 975841db50307c4e2a40d46d6218fc9c8641792e
parks.html        a299c290b6d558f7ce15e337a43cbd04750538be
css/style.css     5497802c6d44cfed1deb161cbb5dd24653874bfc
```
