# TallerdeFedeApp

App web de Taller de Federico: cotizador, presupuestos en PDF, historial de trabajos y métricas.
Es un sitio estático: no necesita instalar ni compilar nada.

## Archivos

- `index.html`: toda la app (pantallas, cálculos y armado del PDF).
- `manifest.webmanifest` e `icons/`: nombre e icono para instalarla en el teléfono.

## Subirla a GitHub

1. Entrá al repositorio `TallerdeFedeApp`.
2. Agregar archivo (Add file) > Subir archivos (Upload files).
3. Arrastrá `index.html`, `manifest.webmanifest`, `README.md` y la carpeta `icons`.
4. Confirmar cambios (Commit changes).

## Publicarla en Cloudflare Pages

1. En Cloudflare: Workers y Pages (Workers & Pages) > Crear (Create) > Pages > Conectar a Git (Connect to Git).
2. Elegí el repositorio `TallerdeFedeApp`.
3. Preajuste de framework (Framework preset): Ninguno (None).
4. Comando de compilación (Build command): dejalo vacío.
5. Directorio de salida (Build output directory): `/`
6. Guardar e implementar (Save and Deploy).

Cada vez que subas una versión nueva a GitHub, Cloudflare la publica sola.

## Datos

Los datos se guardan en el navegador del dispositivo donde se usa (localStorage).
Todavía no hay sincronización con Firebase: usá Configuración > Copia de seguridad
para descargar los datos y restaurarlos en otro dispositivo.
