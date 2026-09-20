# Tarea 2: Selectores avanzados y visualización

Esta carpeta contiene una copia modificada de las tres páginas de la Tarea 1 de `ecpachecop-bit/WD4E-Intro_to_CSS3`. Tiene su propia hoja de estilos y no modifica los HTML ni el CSS de `CSS-week1-HW1`.

## Publicar sin reemplazar la Tarea 1

1. Extrae el ZIP. Dentro encontrarás la carpeta `CSS-week2-HW2`.
2. Abre la página principal de tu repositorio: `https://github.com/ecpachecop-bit/WD4E-Intro_to_CSS3`.
3. Sitúate en la raíz, donde se ven todas las carpetas del curso, no dentro de `CSS-week1-HW1`.
4. Pulsa **Add file → Upload files** y arrastra la carpeta completa **CSS-week2-HW2** a la zona de carga. GitHub permite arrastrar carpetas y conserva su estructura.
5. Comprueba que las rutas que vas a guardar empiezan por `CSS-week2-HW2/`. Escribe el mensaje `Agregar Tarea 2: selectores, Grid y Flexbox` y guarda directamente en `main` con **Commit changes**, si esa opción está disponible en tu copia.
6. Conserva la configuración de GitHub Pages que usaste para la Tarea 1: rama `main`, carpeta `/(root)`. Al guardarse cambios en esa rama, Pages vuelve a publicar. Espera a que la ejecución correspondiente en **Actions** termine correctamente.

**No subas el ZIP comprimido. No reemplaces los archivos de la Tarea 1. No metas esta carpeta dentro de otra carpeta del curso.**

La estructura final debe ser:

```text
WD4E-Intro_to_CSS3/
├── CSS-week1-HW1/             ← Se conserva sin cambios.
│   ├── images/               ← Fotografías compartidas.
│   ├── css/style.css         ← Estilos originales de la Tarea 1.
│   ├── index.html
│   ├── neighborhood.html
│   └── parks.html
└── CSS-week2-HW2/             ← Carpeta nueva que debes subir.
    ├── css/style.css         ← Única hoja de estilos de la Tarea 2.
    ├── index.html
    ├── neighborhood.html
    ├── parks.html
    ├── README.md
    └── VERIFICACION.md
```

## Fotografías: no es necesario subirlas otra vez

Las nuevas páginas reutilizan las fotografías que ya existen en tu repositorio. Las rutas son relativas, por ejemplo:

```html
<img src="../CSS-week1-HW1/images/BaconGallupPark.jpg" alt="Brown Labradoodle sitting next to a statue.">
```

El ZIP contiene las páginas, el CSS y estas instrucciones, **no las fotografías**. Por eso `CSS-week2-HW2` debe quedar al mismo nivel que `CSS-week1-HW1`.

Para abrir el proyecto en el computador con las fotografías, coloca ambas carpetas una junto a otra y conserva `CSS-week1-HW1/images`. Abrir solo este ZIP extraído, sin la carpeta de imágenes de la Tarea 1, no mostrará las fotografías. Esto no exige modificar los archivos originales.

## Requisitos implementados

| Requisito | Implementación |
|---|---|
| Copia nueva del trabajo anterior | Carpeta `CSS-week2-HW2`, con tres HTML y CSS independiente. |
| Hoja de estilos compartida | Los tres HTML enlazan a `css/style.css` dentro de la carpeta nueva. |
| Saltar al contenido principal | Primer enlace del `body`, `href="#main-content"`; destino `<main id="main-content" tabindex="-1">`. |
| Idioma del enlace de salto | Texto español con `lang="es"`; el contenido original restante sigue en inglés. |
| Comentar el estilo de `li` | Están comentadas la regla original y la regla móvil. No hay otra regla activa para `li`. |
| Navegación `inline-block`, 80% | `nav { display: inline-block; width: 80%; }`. Su padre no es flex ni grid. |
| Imagen de navegación al 10% | La fotografía está realmente dentro de `nav`; se utiliza el selector descendente `nav img`. |
| Rejilla de dos columnas al 40% | `neighborhood.html` usa `.grid` y `grid-template-columns: 40% 40%`. |
| Imágenes de Grid al 100% | `.grid img { width: 100%; }`, sin una regla global que lleve ese ancho a Flexbox. |
| Distribución de Grid | `justify-content: space-evenly`, `align-items: center`, `row-gap: 32px` (20px en móvil). |
| Galería flexible | `parks.html` usa `.flex`, `display: flex`, `flex-wrap: wrap`, `justify-content: space-evenly`. |
| Anchos independientes en Flexbox | 28% en escritorio, 44% en tabletas pequeñas y 90% en móviles. |
| Acceso por teclado | Foco visible, enlace de salto visible al recibir el foco y sin animación obligatoria. |

La consigna compartida no incluía capturas de referencia de la Tarea 2. La distribución sigue las propiedades exigidas; no se presenta como una reproducción exacta de imágenes de ejemplo que no se suministraron.

## Comprobar el enlace de salto

En cada página, recarga, pulsa **Tab** y comprueba que aparezca **Saltar al contenido principal**. Pulsa **Enter**: el destino debe ser `#main-content`, y el foco debe pasar al elemento `main`. El enlace es una función de accesibilidad; no necesita JavaScript.

## Validar antes de entregar

El proyecto tiene pruebas locales documentadas en `VERIFICACION.md`. **Aún no está subido ni publicado por esta entrega, y no tiene un nuevo informe oficial de WAVE o W3C.**

Cuando Pages termine de publicar, revisa estas tres direcciones con WAVE y W3C:

- `https://ecpachecop-bit.github.io/WD4E-Intro_to_CSS3/CSS-week2-HW2/index.html`
- `https://ecpachecop-bit.github.io/WD4E-Intro_to_CSS3/CSS-week2-HW2/neighborhood.html`
- `https://ecpachecop-bit.github.io/WD4E-Intro_to_CSS3/CSS-week2-HW2/parks.html`

Son las direcciones previstas para esta ubicación, no afirmaciones de que ya estén publicadas.

En WAVE revisa especialmente **Errors** y **Contrast Errors**. En W3C comprueba el marcado HTML. Recorre también los enlaces con teclado, comprueba la carga de las fotografías y abre el menú fuera de la herramienta WAVE. Los resultados anteriores de la Tarea 1 no validan automáticamente esta nueva versión.

Después de corregir cualquier error que se detecte, entrega la URL de **index.html** de la Tarea 2 en Coursera y completa **tres revisiones por pares**.

## Procedencia y documentación

Contenido y fotografías originales: Colleen van Lent / material del curso *Web Design for Everybody*. Se conserva la atribución en el pie de las tres páginas. Los HTML y el CSS de partida coinciden con los archivos consultados de tu Tarea 1.

- Base del trabajo: https://github.com/ecpachecop-bit/WD4E-Intro_to_CSS3/tree/main/CSS-week1-HW1
- Añadir archivos o carpetas en GitHub: https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
- Publicar desde una rama en GitHub Pages: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- Técnica de salto al contenido de W3C: https://www.w3.org/WAI/WCAG22/Techniques/general/G1
- WAVE: https://wave.webaim.org/
- W3C: https://validator.w3.org/
