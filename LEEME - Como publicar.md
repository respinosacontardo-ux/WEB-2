# Cómo publicar el sitio de MKT BATTISTON con GitHub Pages

Este paquete contiene el sitio web ya listo para publicar. Solo tenés que
subirlo a un repositorio de GitHub y activar GitHub Pages. Son 3 pasos:

## Paso 1 — Subir los archivos al repositorio

1. Entrá a tu repositorio en GitHub (por ejemplo `respinosacontardo-ux/web`)
2. Tocá el botón **"Add file" → "Upload files"** (o "Agregar archivo → Cargar archivos")
3. Arrastrá la carpeta **`docs`** completa (con todo lo que tiene adentro)
   a la zona de carga
4. Abajo tocá el botón verde **"Commit changes"** (Confirmar cambios)

> Importante: tiene que quedar la carpeta `docs` en el repositorio, con
> `index.html` y la carpeta `assets` adentro. Así:
>
> ```
> tu-repositorio/
> └── docs/
>     ├── index.html
>     └── assets/
>         ├── index-CN6ge7iX.css
>         └── index-Jqy1LVt2.js
> ```

## Paso 2 — Activar GitHub Pages

1. En el repositorio, andá a **Settings → Pages** (Configuración → Páginas)
2. En **Source** (Fuente) elegí **"Deploy from a branch"**
   (Implementar desde una rama)
3. En **Branch** (Rama) elegí **`main`** (puede aparecer como "principal")
4. En la carpeta elegí **`/docs`** (puede aparecer traducido como "/documentos")
5. Tocá **Save** (Guardar / "Ahorrar")

## Paso 3 — Ver tu sitio online

Esperá 1 a 5 minutos y tu sitio va a estar disponible en:

```
https://TU-USUARIO.github.io/NOMBRE-DEL-REPOSITORIO/
```

Por ejemplo, si lo subís al repositorio `web`:
`https://respinosacontardo-ux.github.io/web/`

La dirección exacta aparece arriba de todo en la misma pantalla de
Settings → Pages una vez que se publica.

## ¿Querés cambiar algo del sitio más adelante?

El código fuente (para editar textos, colores, secciones, etc.) está en el
repositorio `EDITOR-DE-VIDEOS`, rama `claude/mkt-battiston-website-aizeaq`,
carpeta `mkt-battiston-website`. Los textos se editan en un solo archivo:
`src/data/content.js`. Después de cualquier cambio hay que volver a compilar
(`npm run build`) y reemplazar el contenido de `docs` con el resultado.

---
MKT BATTISTON — Software de automatización con IA para redes sociales
