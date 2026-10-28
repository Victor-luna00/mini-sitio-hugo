---
title: "Desplegando Hugo con Nginx en Debian (SRI P1.2)"
date: 2026-10-28
draft: false
---

En la práctica de SRI P1.2 hemos dado el salto del servidor de desarrollo (`hugo server`) a un servidor web de producción real con **Nginx**:

- Compilación de los archivos estáticos mediante el comando `hugo` hacia la carpeta `public/`.
- Instalación de Nginx en nuestra máquina virtual Debian 13.
- Configuración de un VirtualHost en `/etc/nginx/sites-available/mi-sitio`.
- Comprobación de conectividad mediante IP y resolución con `/etc/hosts` simulando un sistema DNS.
