# AGENT.md — Reglas para el agente de IA

Proyecto: **Portfolio Personal Web (Entrega 1)** de Silvina Carolina Carrizo.
Antes de generar o modificar código, el agente debe respetar estas reglas. Si alguna sugerencia las rompe, hay que corregirla antes de entregar.

## Stack permitido
- Solo **HTML5** y **CSS3 puro**.
- **Prohibido Tailwind CSS.** Bootstrap es opcional (en este proyecto NO se usa).
- Sin JavaScript en esta entrega.

## Archivos y carpetas
- `index.html` → única página (One Page / Landing Page).
- `styles.css` → única hoja de estilos, vinculada con `<link rel="stylesheet" href="styles.css">`.
- `assets/` → todo lo multimedia (imágenes en `assets/img/`, fuentes, videos).
- No mezclar estilos dentro del HTML (nada de atributos `style=""` ni etiquetas `<style>`).

## Reglas de HTML
- `<!DOCTYPE html>`, `<html lang="es">`, `<meta charset="utf-8">`, meta viewport y `<title>` descriptivo.
- Estructura semántica: `<header>` con `<nav>` → `<main>` único → `<footer>`.
- `<main>` tiene exactamente 4 `<section>`, cada una con su `<h2>`:
  1. `id="sobre-mi"` — presentación + `<img>` con `alt` descriptivo.
  2. `id="skills"` — habilidades en listas `<ul>`/`<li>` (sin párrafos largos).
  3. `id="proyectos"` — cada proyecto dentro de un `<article>` con título, descripción, imagen previa y enlaces externos.
  4. `id="contacto"` — `<form>` con cada `<label for="x">` vinculado a su `<input id="x">` + enlaces directos.
- Los enlaces del `<nav>` son internos: `href="#id-seccion"`.
- Todo enlace externo lleva `target="_blank"` y `rel="noreferrer"`.
- Todas las imágenes llevan `alt` descriptivo.
- Un solo `<h1>` en toda la página. Jerarquía de títulos ordenada (h1 → h2 → h3).
- El `<footer>` incluye © y enlaces secundarios.

## Reglas de CSS (orden estricto del archivo)
1. **Reset y variables:** `* { margin: 0; padding: 0; box-sizing: border-box; }` y `:root` con colores y tipografías.
2. **Estilos por sección:** bloques comentados, usando **clases reutilizables** (`.contenedor`, `.seccion`, `.titulo-seccion`, `.boton`, `.tarjeta`, `.chip`).
3. **Responsive al final:** todas las `@media` van al final del archivo, nunca en el medio.

- Maquetación con **Flexbox y/o CSS Grid** (menú, tarjetas, grillas).
- Combinar unidades fijas (`px`) y relativas (`rem`, `%`, `vh`, `vw`).
- Usar siempre las variables de `:root` para colores y fuentes; no escribir colores sueltos.
- No usar `!important`.

## Convenciones
- Nombres de clases en español y en minúscula, con formato tipo BEM (`bloque__elemento--modificador`).
- Comentar cada bloque del CSS y cada sección del HTML.
- Indentación de 2 espacios.
