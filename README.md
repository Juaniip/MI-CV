# CV Web

Mi portfolio personal. Es el CV de toda la vida pero en forma de página, para no andar mandando un PDF cada vez que alguien me pide el currículum.

Todo el sitio vive en un solo archivo, `index.html`. HTML, CSS y JS metidos adentro, sin frameworks ni build. Lo elegí así para no complicarme con un paso de build al deployar: se sube tal cual y funciona.

La única dependencia es [anime.js](https://animejs.com) (v4.5.0, MIT) para las animaciones, y está copiada en `js/anime.umd.min.js` (el bundle UMD, así también anda abriendo el HTML directo con `file://`). Para actualizarla, se reemplaza ese archivo por el `dist/bundles/anime.umd.min.js` de una versión nueva. Si el navegador pide reducir movimiento, o si el script no carga, el sitio se muestra completo sin animaciones.

## Verlo local

Se puede abrir `index.html` directo en el navegador, o si querés levantarlo con un servidor:

```
npx serve .
```

## Actualizar el contenido

Todo el HTML está ahí adentro, secciones bien separadas (educación, experiencia, proyectos, etc.). Para agregar algo nuevo —un trabajo, un curso— es cuestión de buscar la sección correspondiente y sumar el bloque.

## Deploy

Vive en Cloudflare Pages con dominio propio.
