# INCOEX · App móvil en HTML (20 pantallas)

Proyecto **estático, sin instalación ni build** para GitHub Pages. Incluye `index.html` (login), `pantallas.html` (selector de pantallas) y **20 HTML independientes**, cada uno con su `<style>` y `<script>` embebidos. El diseño es responsivo y optimizado para pantallas de teléfono. Los archivos están conectados mediante links, botones y localStorage.

## Publicación en GitHub Pages
1. Extraé todo el ZIP.
2. Subí **el contenido de la carpeta** a la raíz de un repositorio público (incluyendo `index.html` y la carpeta `assets/`).
3. En GitHub, abrí **Settings → Pages → Build and deployment → Deploy from a branch**; elegí la rama `main` y `/ (root)`.
4. Abrí el enlace que GitHub proporciona. `index.html` se ejecuta automáticamente.

## Imágenes e iconos
Están deliberadamente vacíos. Solo tenés que guardar tus imágenes con los nombres exactos de `assets/README_IMAGENES.txt`. El HTML ya contiene sus rutas. También podés editar las etiquetas `src="assets/..."` en cada archivo. Los iconos se esperan en `assets/icons/*.svg` y tienen un marcador de reserva mientras falten.

## Navegación y demo
- Inicio de sesión y registro con campos locales; no hay autenticación real.
- Selección de recogida, destino, vehículo, pasajeros, método de pago, confirmación, búsqueda, recorrido y cierre del viaje.
- Inicio, viajes, historial, billetera y perfil enlazados.
- Las selecciones se guardan en `localStorage` en el navegador para atravesar las pantallas.
- Mapa, conductor, geolocalización, pago, recarga, chat y tracking se simulan: **no llaman a servicios reales**.
- Para comprobar todas las pantallas usá `pantallas.html`.

## Limitación de fidelidad
La referencia de 20 pantallas llegó como una sola imagen de apenas **759 × 96 px**. No es posible leer textos, iconos ni medidas exactas desde esa resolución. Por ello esta entrega replica la **paleta, estructura móvil, gradientes, paneles y flujo visual de referencia** con una interpretación de la jerarquía. Para una réplica píxel por píxel, necesitaremos capturas individuales de alta resolución.

## Uso del código
Cada archivo es autónomo en HTML, CSS y JavaScript, sin librerías ni CDN, por lo que puede compartirse individualmente si va acompañado de sus imágenes opcionales. Para cambiar el flujo, buscá `data-go="archivo.html"` o las opciones `data-action` en cada página.
