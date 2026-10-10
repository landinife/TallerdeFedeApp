# TallerdeFedeApp

App web de Taller de Federico: cotizador, presupuestos en PDF, historial de trabajos y métricas.
Es un sitio estático: no necesita instalar ni compilar nada.

## Archivos

- `public/index.html`: toda la app (pantallas, cálculos y armado del PDF).
- `public/manifest.webmanifest` y `public/icons/`: nombre e icono para instalarla en el teléfono.
- `wrangler.jsonc`: le indica a Cloudflare que publique la carpeta `public`.

## Publicarla en Cloudflare

1. En Cloudflare: Workers y Pages (Workers & Pages) > Crear (Create) > Importar un repositorio (Import a repository).
2. Elegí el repositorio `TallerdeFedeApp`.
3. Dejá las opciones como vienen: el archivo `wrangler.jsonc` ya indica qué publicar.
4. Guardar e implementar (Save and Deploy).

Cada vez que se sube una versión nueva a GitHub, Cloudflare la publica sola.

## Datos

Los datos se guardan en el navegador del dispositivo donde se usa (localStorage).
Todavía no hay sincronización con Firebase: usá Configuración > Copia de seguridad
para descargar los datos y restaurarlos en otro dispositivo.
