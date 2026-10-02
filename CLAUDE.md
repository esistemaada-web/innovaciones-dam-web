# CLAUDE.md — Innovaciones DAM (página web)

Instrucciones para Claude Code al trabajar en este repo. Se lee automáticamente
al iniciar sesión.

## Qué es esto

Página web de una sola pantalla (`index.html`, sin build) con los servicios de
**Innovaciones DAM / Sistema ADA**, desplegada en Vercel. Pensada para que los
clientes vean la oferta de servicios y puedan contactar por WhatsApp o correo.

## "respaldo" — al terminar cambios

Cuando el usuario diga **"respaldo"**, hacerlo **sin pedir confirmación**:

1. **Git** — `git add` solo los archivos tocados de la página (nunca tokens ni
   credenciales); `git commit` con mensaje descriptivo en español, terminando con
   `Co-Authored-By: Claude Sonnet 5 <noreply@anthropic.com>`.
2. **GitHub** — `git push` a `main` del repo `esistemaada-web/innovaciones-dam-web`.
3. **Vercel** — el proyecto está conectado al repo, así que el push dispara el
   redeploy solo; no hace falta ejecutar nada manual. Avisar al usuario que
   revise `https://innovaciones-dam-web.vercel.app/` en 1-2 minutos para
   confirmar que tomó los cambios. Si el build de Vercel falla, avisar.

Si `git push` falla por conflicto o hay cambios remotos que chocan: avisar, NO
forzar (nada de `push --force` sin permiso explícito).

## Convenciones

- Sitio estático sin build: los cambios de contenido o diseño se hacen directo
  en `index.html` (HTML + CSS + JS inline, sin frameworks).
- Datos de contacto en la página: WhatsApp **+58 424 567 3867**, correo
  **esistemaada@gmail.com**. Si cambian, actualizar los enlaces `wa.me` y
  `mailto:` en `index.html` y este archivo.
- El usuario escribe en español → responder en español.
- Dominio de producción en Vercel: `innovaciones-dam-web.vercel.app`.
