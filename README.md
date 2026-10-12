# DimeloGasp · Portfolio

Portfolio web de **Gaspar Navarro (DimeloGasp)**, productor musical de Mar del Plata, Argentina.
Beats, mezcla, Auto-Tune en vivo y sonido técnico para shows de música urbana.

Sitio estático en un solo archivo (HTML, CSS y JavaScript sin dependencias ni paso de compilación), con diseño inspirado en el portfolio de Dennis Snellenberg.

## Secciones

- **Portada**: foto a sangre, nombre gigante en movimiento y rol.
- **Sobre mí**: presentación y cifras animadas.
- **Música**: reproductor de Spotify con la playlist completa de temas producidos.
- **Servicios**: producción y beats, mezcla, Auto-Tune en vivo, sonido y live rig.
- **Artistas y colaboraciones**: Omar Varela destacado y el resto de los artistas en cintas animadas.
- **En vivo**: escenarios de Mar del Plata donde trabajó.
- **Herramientas**.
- **Fotos**: galería con visor ampliado (flechas y teclado).
- **Contacto**: botón directo a WhatsApp e Instagram.

## Efectos

- Pantalla de carga con saludos.
- Cursor personalizado con anillo elástico y estela (solo en dispositivos con mouse).
- Textos que aparecen palabra por palabra al hacer scroll.
- Marquesinas que cambian de sentido y aceleran con el scroll.
- Parallax en fotos, botones magnéticos y menú lateral fijo.
- Diseño adaptado a celulares.

## Estructura

```
.
├── index.html              # todo el sitio: estructura, estilos y scripts
└── assets/
    └── img/
        ├── perfil/
        │   └── perfil.jpg
        └── proyectos/
            ├── vivo-01.jpg ... vivo-05.jpg
```

## Verlo en tu compu

El reproductor de Spotify necesita que la página se sirva desde un servidor (con doble clic puede quedar en blanco). Desde la carpeta del proyecto:

```bash
python -m http.server 5510
```

Después abrí `http://localhost:5510` en el navegador.

## Publicarlo con GitHub Pages

1. Subí el contenido de esta carpeta a un repositorio de GitHub.
2. En el repositorio, entrá a **Settings → Pages**.
3. En **Source** elegí **Deploy from a branch**, la rama `main` y la carpeta `/ (root)`.
4. Guardá. En un par de minutos el sitio queda en `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

También funciona tal cual en Vercel, Netlify o cualquier hosting estático (Hostinger, etc.): solo hay que subir los archivos.

## Cómo editar el contenido

Todo se cambia en `index.html`:

| Qué | Dónde buscar |
| --- | --- |
| Número y mensaje de WhatsApp | `var WA = "https://wa.me/...` (en el script, al final) |
| Playlist de Spotify | `open.spotify.com/embed/playlist/...` (sección `#musica`) |
| Instagram | `instagram.com/dimelogasp_` |
| Cifras | atributos `data-count` en el bloque `facts` |
| Fotos de la galería | sección `#fotos`, etiquetas `<img src="assets/img/proyectos/...">` |
| Colores | variables `--accent`, `--bg` y `--deep` al inicio del `<style>` |

Para agregar una foto nueva a la galería, guardala en `assets/img/proyectos/` (JPG, idealmente menos de 500 KB) y copiá uno de los bloques `<figure>` de la sección `#fotos` cambiando la ruta y el texto `alt`.

## Contacto

- WhatsApp: [+54 9 223 550-3325](https://wa.me/5492235503325)
- Instagram: [@dimelogasp_](https://www.instagram.com/dimelogasp_/)
- Spotify: [Produced w Dimelo Gasp](https://open.spotify.com/playlist/1HtE5mrDMdr6NBlzEh76Ow)

---

© 2026 Gaspar Navarro. Todos los derechos reservados sobre fotos, música y marca.
