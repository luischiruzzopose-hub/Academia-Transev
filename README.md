# TRANSEV — Sitio web

Sitio estático (HTML/CSS/JS, sin build ni dependencias) de la Academia de Choferes TRANSEV.

## Estructura
```
index.html         → página principal
simulacro.html      → simulador de examen teórico
styles.css / script.js
assets/
  images/            fotos del sitio
  images/simulacro/  señales de tránsito del simulador
  video/             video testimonio
  docs/              manual en PDF
  icons/             íconos svg
```

## Subir esto a GitHub (primera vez)

1. Instalá Git si no lo tenés: https://git-scm.com/downloads
2. Creá un repositorio nuevo y vacío en https://github.com/new (por ejemplo `transev-web`). NO le tildes "Add a README".
3. Abrí una terminal dentro de esta carpeta (`transev-web`) y corré:

```bash
git init
git add .
git commit -m "Sitio TRANSEV"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/transev-web.git
git push -u origin main
```

Reemplazá `TU-USUARIO` por tu usuario de GitHub.

## Publicarlo gratis con GitHub Pages

1. En GitHub, entrá al repositorio → **Settings** → **Pages**.
2. En "Source" elegí la rama `main` y la carpeta `/ (root)`.
3. Guardá. En unos minutos el sitio queda online en:
   `https://TU-USUARIO.github.io/transev-web/`

## Actualizar el sitio más adelante

Cada vez que quieras subir cambios nuevos:
```bash
git add .
git commit -m "Descripción del cambio"
git push
```

## Nota sobre el simulacro

En `simulacro.html`, dos preguntas del banco de señales ("curva peligrosa a la
izquierda" y "hospital") no tenían foto real disponible; una ya fue reemplazada
por una pregunta nueva. La otra (curva peligrosa a la izquierda) sigue mostrando
"Imagen no disponible" hasta que se agregue la señal correspondiente en
`assets/images/simulacro/curva-peligrosa-izquierda.svg`.
