CIMAC — Home / build de producción
===================================

Contenido
---------
index.html                 Página completa (home)
support.js                 Runtime que renderiza la página. Debe quedar junto a index.html.
_ds/industry-.../          Hoja de estilos y bundle del design system Industry
assets/fonts/              Euclid Flex (.ttf) y Campton (.otf)
assets/team/               Fotos del equipo
assets/hero-comp5.mp4      Video del hero
assets/*.png               Logos (CIMAC, USACH, ANID, Ministerio, consorcio) y fondos

Cómo publicarlo
---------------
1. Subir TODO el contenido de esta carpeta al servidor, manteniendo la
   estructura de carpetas tal cual (index.html en la raíz del sitio).
2. Servir por HTTP/HTTPS. Abrir el archivo con doble clic (file://) no
   funciona: el navegador bloquea la carga de los assets.
3. No hay build ni dependencias de node. Es hosting estático
   (Netlify, Vercel, S3, Apache, Nginx, cPanel, etc.).

Dependencia externa
-------------------
El scroll suave usa Lenis desde CDN:
https://unpkg.com/lenis@1.1.18/dist/lenis.min.js
Si el sitio debe funcionar sin acceso a internet externo, descargar ese
archivo, guardarlo en assets/ y cambiar el <script src> en index.html.

Notas
-----
- El video del hero está silenciado y en autoplay; así lo exigen los
  navegadores para reproducir sin interacción del usuario. No quitar el
  atributo muted.
- Los enlaces de WhatsApp, correo y redes sociales son placeholders:
  revisar y reemplazar por los datos reales antes de publicar.
- Las fuentes Euclid Flex y Campton son de licencia comercial.
  Confirmar que la licencia cubre el uso web antes de publicar.
