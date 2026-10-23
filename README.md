# INCOEX · V3 Glass iPhone — 21 pantallas HTML independientes

**Esta es la versión nueva:** no mezclar archivos con ZIP anteriores; eliminar los antiguos del repositorio antes de subir estos.

## Navegación
1. `index.html` inicia en Login; registro funciona con validación local.
2. Desde Inicio: transporte → mapa → programación → vehículo → detalles → seleccionar servicio → ubicaciones → paradas → adicionales → tarifa → confirmar → buscando → conductor → finalizar.
3. Dock flotante estilo Liquid Glass en Inicio, Viajes, Resumen y Perfil. Todos sus enlaces apuntan a archivos existentes.
4. `pantallas.html` muestra la **galería de iframes con las páginas verdaderas**. Abrí este archivo para ver las 21 vistas al mismo tiempo.

## GitHub Pages
- Subí el contenido DESCOMPRIMIDO del ZIP en la raíz del repositorio (`index.html` visible al mismo nivel que las 21 páginas).
- Settings > Pages > Deploy from a branch > main > /(root).
- No requiere Node, npm, API, CDN ni framework. HTML, CSS y JavaScript están DENTRO DE CADA .html.

## Reemplazar imágenes e íconos
En `assets/GUIA_IMAGENES.txt` están los nombres esperados. Poné PNG de tus mascotas, motos, banners y mapas, reemplazando placeholders. Los íconos del menú inferior son SVG inline (cambiarlos en cada HTML o por tus SVG propios). Los demás iconos usan `assets/icons/*.svg` con glifos de respaldo.

## Estado funcional local
- Formularios con comprobación de campos/contraseña, selección de servicio y vehículo, horarios personalizados, recogida/destino, paradas, cantidad, adicionales, pago, filtros, estadísticas, puntuación, perfil, registro de viaje de prueba.
- Los datos se conservan con `localStorage` al cambiar páginas.
- No existe backend: no hay autenticación real, pago, GPS, rastreo ni asignación de conductores. Toda esa parte está simulada y requiere API para producción.

## Diseño
- Referencia visual del usuario: 21 pantallas en grid. Recreación en móvil, no pixel-perfect sin imágenes originales.
- El menú es un dock flotante translúcido con blur, brillo, borde y reflejos tipo Liquid Glass, NO un navbar sólido.
- Cada pantalla es responsive (360–430 px de base) y se adapta al móvil/desktop.
