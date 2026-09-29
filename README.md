# Cabeza coronada

Instalación 3D interactiva: una cabeza policromada con diadema de plata y un Sagrado Corazón, cada uno sobre una columna de mármol tallada, frente a dos láminas planas (el retablo dorado y la Virgen con ángeles).

## Contenido

| Archivo | Qué es |
|---|---|
| `index.html` | Visor web interactivo (three.js). Vistas de conjunto, cabeza y figura; luz ajustable. |
| `modelo/instalacion.glb` | Escena completa en 3D (esculturas, columnas y láminas) para Blender, Sketchfab, etc. |
| `imagenes/` | Texturas y láminas que usa el visor. |

## Ver el visor en tu computadora

Abrir `index.html` directamente puede no cargar la textura por restricciones del navegador. Levantá un servidor local desde esta carpeta:

```bash
python3 -m http.server 8000
```

y abrí http://localhost:8000

## Publicarlo con GitHub Pages

1. Subí este repositorio a GitHub.
2. En el repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Elegí la rama `main` y la carpeta `/ (root)`, y guardá.
4. En uno o dos minutos queda online en `https://TU-USUARIO.github.io/cabeza-coronada/`.

## Notas sobre la reconstrucción

Ambas esculturas se reconstruyeron a partir de una única fotografía frontal. En la cabeza, los laterales y la parte posterior son interpretación; el Sagrado Corazón es un relieve de bulto generado desde la silueta y el sombreado de la foto, con el dorso en colores del manto. En el `.glb` la plata es un material metálico: se ve plateada en visores con iluminación de entorno (HDRI); en visores sin entorno puede verse oscura.
