# INCOEX — Prototipo HTML responsive, 21 pantallas

## Instalación y GitHub Pages
1. Descomprime el ZIP y sube **todo** a la raíz de tu repositorio (incluyendo `assets/`).
2. GitHub → Settings → Pages → Deploy from branch → `main` → `/ (root)`.
3. Abre `index.html` para la aplicación o `pantallas.html` para revisar las 21 pantallas.

## Contenido
- 21 archivos HTML, CSS y JavaScript **dentro de cada HTML**, sin CDN.
- Interfaz responsive para anchos 320–430 px, con vista previa en escritorio.
- Barra inferior estilo Liquid Glass, y navegación enlazada.
- Servicios: moto delivery, automóvil pasajeros, SUV pasajeros, furgón carga mediana, camión carga pesada.
- 5 vehículos del usuario en `assets/` como PNG y versiones WebP optimizadas. Copias originales en `assets/originales/`.
- Marcadores/iconos SVG editables en `assets/icons/`.
- Mapa de diseño **ilustrativo** en `assets/mapa-managua.png`, no usa localización real.
- Login, estado del servicio, horario, dirección, tipo de vehículo, pago y rating son una **demostración local** guardada en localStorage.

## Límites conocidos
Este proyecto se hizo a partir de las capturas e imágenes que entregó el usuario. El enlace Figma indicado no pudo leerse como capas ni obtener su CSS/tokens originales desde las herramientas disponibles; por ello **no es exacto pixel-perfect al archivo Figma**. Para fidelidad total se necesita acceso de lectura a Figma o exportaciones de cada frame y assets faltantes.
Los importes y tiempos son ejemplos, no tarifas comerciales reales. No hay pagos, mapa GPS, login real, driver dispatch ni back-end.

## Modificar imágenes
Las fotos ya están añadidas (moto, carro, SUV, furgón y camión). Sustituye las imágenes en `assets/` conservando el nombre del archivo. Para editar iconos, modifica SVG de `assets/icons/`.
