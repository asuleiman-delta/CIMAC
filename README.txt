CIMAC — home (build de producción)
==================================

Contenido
  index.html   la home completa
  support.js   runtime que la renderiza (debe quedar junto a index.html)
  _ds/         hoja de estilos y bundle del sistema de diseño
  assets/      video del hero, fotos, logos, fuentes, ícono de WhatsApp

Cómo publicarla
  Sube el contenido de esta carpeta a la raíz del hosting, tal cual
  (index.html arriba, y las carpetas assets/, _ds/ al mismo nivel).
  Es un sitio estático: sirve en cualquier hosting o CDN, sin build.

Notas
  · Debe servirse por http/https, no abriendo el archivo con doble clic.
  · React se carga desde unpkg.com; si necesitas que funcione sin internet,
    hay que vendorizar esas dos librerías.
  · El video del hero pesa la mayor parte del build: si el sitio queda
    lento en móvil, comprímelo o cámbialo por uno más corto.
  · Pendientes de contenido: el número de WhatsApp (wa.me/56200000000) y
    los correos/enlaces del formulario y footer son de ejemplo.
