# incba-redes

Página "link in bio" de INCBA → **https://redes.incba.com.ar**

Es un solo `index.html` estático, sin dependencias ni paso de compilación. Pesa unos 15 KB más el avatar (4 KB).

## Cómo editar

Todo está en `index.html`, en el bloque marcado **LINKS**:

- **Cambiar un link:** editá el `href` del `<a>` que corresponda.
- **Sacar un link:** borrá su `<a>` completo.
- **Agregar uno:** copiá un `<a class="btn">` existente y cambiale el texto y el `href`.
- **El destacado** es el `<a class="btn btn--destacado">`, hoy "Agendá tu diagnóstico gratuito", que lleva a Calendly.
- **Facebook e Instagram** están más abajo, en `<nav class="redes">`, como íconos.

Los colores están arriba, en `:root` (`--accent` es el verde de INCBA y `--navy` el fondo), y son los mismos de incba.com.ar.

## Publicar

Hacé push a `main` y GitHub Pages lo publica solo en alrededor de un minuto.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | La página completa (HTML y CSS) |
| `img/avatar.webp` | Avatar: el logo de INCBA sobre fondo azul noche |
| `img/favicon-32.png`, `img/apple-touch-icon.png` | Íconos: la "A" de INCBA |
| `img/og-image.jpg` | Imagen de vista previa al compartir el link (la misma de la web) |
| `CNAME` | Dominio propio para GitHub Pages |
| `.nojekyll` | Le dice a GitHub Pages que publique los archivos tal cual |

## Dominio

`redes.incba.com.ar` es un CNAME a `incba.github.io` en Cloudflare, en modo **DNS only** (nube gris), igual que `incba.com.ar`. Así GitHub emite el certificado HTTPS.

## Números de WhatsApp

Son los mismos que publican las webs: Argentina `+54 9 351 742-2702` y Chile `+56 9 5740 0433`. Si querés que los chats de Argentina entren al CRM, cambiá el número de Argentina por el de la línea de WhatsApp del CRM.
