CIMAC — Sitio web / build de producción
=======================================

Contenido
---------
index.html                 Home
noticia.html               Detalle de noticia (?n=1, ?n=2 o ?n=3 elige la noticia)
support.js                 Runtime que renderiza las páginas. Debe quedar junto a los .html.
_ds/industry-.../          Hoja de estilos y bundle del design system
assets/fonts/              Euclid Flex (.ttf) y Campton (.otf)
assets/team/               Fotos del equipo
assets/empresas/           Logos de empresas colaboradoras
assets/ref/                Imágenes de noticias y secciones
assets/hero-comp5.mp4      Video del hero
assets/*.png               Logos institucionales, slides del hero y fondos

Cómo publicarlo
---------------
1. Subir TODO el contenido de esta carpeta al servidor, manteniendo la
   estructura de carpetas (index.html en la raíz del sitio).
2. Servir por HTTP/HTTPS. Abrir con doble clic (file://) no funciona.
3. Sin build ni dependencias de node. Hosting estático
   (Netlify, Vercel, S3, Apache, Nginx, cPanel, etc.).

Dependencia externa
-------------------
El scroll suave usa Lenis desde CDN:
https://unpkg.com/lenis@1.1.18/dist/lenis.min.js
Para funcionar sin internet externo, descargarlo a assets/ y cambiar el
<script src> en index.html y noticia.html.

Notas
-----
- El texto del detalle de noticia es placeholder (igual en las 3);
  solo cambian título, fecha e imagen.
- El video del hero está silenciado y en autoplay. No quitar "muted".
- WhatsApp, correo y redes sociales son placeholders.
- Euclid Flex y Campton son fuentes comerciales: confirmar licencia web.
