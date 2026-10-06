# Innovaciones DAM

Página web de servicios de Innovaciones DAM / Sistema ADA.

Sitio estático de una sola página (`index.html`, sin build), listo para
desplegar en Vercel sin configuración adicional.

## Servicios mostrados

- Digitalización
- Automatización
- Redes Sociales
- Sistemas Informáticos
  - Sistema ADA
  - Sistema iADA (RAG, Reportes Personalizados, App_Respaldo)

## Agendar cita

Sección `#agendar`: formulario (nombre, medio preferido — llamada telefónica /
WhatsApp / videollamada —, fecha y hora) que arma un mensaje de WhatsApp con
la solicitud. No hay backend ni calendario externo conectado; si más adelante
se consigue un enlace de Google Calendar o Calendly, se puede reemplazar por
un calendario embebido real.

## Contacto en la página

- WhatsApp: +58 424 567 3867 (variable `WA_NUMBER` en el `<script>` de `index.html`)
- Correo: esistemaada@gmail.com

## Desarrollo local

No requiere instalación. Abre `index.html` en el navegador, o sirve la
carpeta con cualquier servidor estático, por ejemplo:

```bash
npx serve .
```
