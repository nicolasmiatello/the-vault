# THE VAULT — Sala NBA

Sitio de venta de cartas coleccionables NBA. Es un sitio estático: no necesita instalar nada ni compilar. Todo el sitio está en `index.html` y las fotos y videos en `img/`.

## Qué hay en esta carpeta

| Archivo | Qué es |
|---|---|
| `index.html` | El sitio completo (hall, Sala NBA, vitrina, combos, buscador, pizarra táctica). |
| `img/` | Fotos de las cartas, videos de las puertas de las salas y la intro. |
| `vercel.json` | Configuración de Vercel (URLs limpias y caché de imágenes). |

## Subirlo a GitHub (desde el navegador, sin programas)

1. Entrá a github.com y creá un repositorio nuevo: botón **New**, nombre por ejemplo `the-vault`. Podés dejarlo **Private**.
2. En el repositorio vacío, hacé clic en **uploading an existing file**.
3. Arrastrá **todo el contenido** de esta carpeta (no la carpeta en sí): `index.html`, `README.md`, `vercel.json`, `.gitignore` y la carpeta `img`.
   - `.gitignore` es un archivo oculto. Si no lo ves en tu compu, no pasa nada: no es necesario.
4. Abajo, en **Commit changes**, poné un mensaje como "Primera versión" y confirmá.

Ningún archivo pasa los 25 MB y son menos de 100, así que entra en una sola subida.

## Publicarlo en Vercel

1. Entrá a vercel.com e iniciá sesión con tu cuenta de GitHub.
2. **Add New → Project** y elegí el repositorio `the-vault`.
3. En **Framework Preset** dejá **Other**. No hace falta tocar nada más: sin build command, sin output directory.
4. **Deploy**. En menos de un minuto te da una dirección tipo `the-vault-xxxx.vercel.app`.

Desde ahí, cada vez que subas un cambio al repositorio, Vercel lo publica solo.

## Después del primer deploy

- **Vista previa al compartir el link**: en `index.html`, buscá `TU-DOMINIO` (aparece en dos líneas cerca del principio) y reemplazalo por tu dirección real, por ejemplo `the-vault-xxxx.vercel.app`. WhatsApp y las redes necesitan la dirección completa de la imagen para mostrar la vista previa.
- **Dominio propio**: en Vercel, **Settings → Domains** del proyecto. Si cambiás de dominio, actualizá también las dos líneas de `TU-DOMINIO`.

## Cómo sumar cartas nuevas

Igual que hasta ahora: pasale a Claude las fotos y los datos, y te devuelve el `index.html` actualizado y las fotos nuevas para `img/`. Las subís a GitHub (con **Add file → Upload files**, reemplazando `index.html`) y Vercel publica solo.

## Notas

- El carrito, favoritos y comparador se guardan en el navegador de cada visitante. No hay base de datos.
- Las consultas de compra van por WhatsApp al dueño de cada carta.
