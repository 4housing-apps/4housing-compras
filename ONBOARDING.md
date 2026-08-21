# Onboarding — 4housing-compras

Bienvenida 👋 Esta guía te deja lista para trabajar en el proyecto con Claude Code.

## Qué es este proyecto

Es la app interna **"4housing Operaciones — Compras & Ops"**. Toda la aplicación vive
en un único archivo `index.html` (HTML, CSS y JavaScript embebidos, en español).

- **No hay dependencias que instalar** (no usa npm, ni framework).
- **No hay paso de build.**
- **No hay tests automatizados** todavía.

## Cómo correrla

La forma más simple: abrí `index.html` directamente en el navegador
(doble clic, o arrastralo a una pestaña de Chrome/Edge).

Si preferís servirla desde un servidor local (recomendado si algo carga fuentes o
datos por red), desde la carpeta del proyecto:

```bash
# Con Python (ya viene en la mayoría de los sistemas)
python -m http.server 8000
# luego abrí http://localhost:8000 en el navegador
```

En Windows, si tenés Node instalado, también sirve:

```bash
npx serve .
```

## Estructura

```
4housing-compras/
├── index.html   # Toda la app (UI de Compras & Ops)
└── README.md
```

## Flujo de trabajo con git

1. Traé lo último de `main`:
   ```bash
   git checkout main
   git pull origin main
   ```
2. Creá una rama para tu cambio:
   ```bash
   git checkout -b mica/mi-cambio
   ```
3. Hacé el cambio, probalo en el navegador, y commiteá:
   ```bash
   git add index.html
   git commit -m "Descripción clara del cambio"
   git push -u origin mica/mi-cambio
   ```
4. Abrí un Pull Request en GitHub hacia `main`.

## Tips para trabajar con Claude Code

- Pedile a Claude que te explique una sección antes de tocarla: como todo está en
  un solo archivo, conviene ubicar bien el bloque (buscá por el texto de la pantalla,
  el nombre de una clase CSS, o el rótulo del botón).
- Pedile que corra un servidor local y saque una captura para verificar los cambios.
