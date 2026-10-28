# IAW - P1.2 & SRI - P1.2: Mi Mini Sitio Web con Hugo + Nginx

Este repositorio contiene la entrega de las prácticas de **Implantación de Aplicaciones Web (IAW)** y **Servicios de Red e Internet (SRI)** para 2º de ASIR.

## Estructura del proyecto
- `hugo.toml`: Configuración principal de Hugo.
- `layouts/`:
  - `index.html`: Plantilla principal (Home).
  - `partials/`: Fragmentos reutilizables (`head.html`, `header.html`, `footer.html`).
  - `_default/`: Plantillas para páginas (`single.html`) y listados (`list.html`).
- `content/`:
  - `_index.md`: Contenido de la página de inicio.
  - `sobre-mi.md`: Información personal y enlace al perfil de GitHub (P1.1).
  - `blog/`: Sección de blog con artículos técnicos.
- `static/css/style.css`: Estilos visuales minimalistas (filosofía KISS).

## Instrucciones de uso

### En desarrollo (Hugo Server)
```bash
hugo server -D --watch
```
Acceder en el navegador a: `http://localhost:1313/`

### En producción (Nginx)
Compilar sitio estático:
```bash
hugo
```
Los archivos compilados se generarán en la carpeta `public/`.
Nginx se encarga de servir esta carpeta en el puerto 80.
