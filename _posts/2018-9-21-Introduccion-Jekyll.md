---
layout: post
title: Introducción a Jekyll
---

**Jekyll** es un generador de sitios estáticos perfecto para blogs alojados en GitHub. ([Repositorio de Jekyll](https://github.com/jekyll/jekyll))

![Caputra de pantalla de Jekyll Now](/images/jekyll-now-theme-screenshot.jpg "Caputra de pantalla de Jekyll Now")

## Inicio rápido

### Paso 1) Hacer un fork de Jekyll Now a nuestro repositorio.

Hicimos fork del repositorio, entonces renombramos el repositorio a softwarebeasts.github.io.

![Paso 1](/images/step1.gif "Paso 1")

### Paso 2) Personalizar y ver el sitio

Ingresamos el nombre de nuestro sitio, la descripción, el avatar y muchas otras opciones editando el archivo _config.yml. Aquí también se pueden activar fácilmente el seguimiento de Google Analytics, los comentarios de Disqus y los iconos de redes sociales.

Haciendo un cambio en _config.yml (o cualquier archivo en el repositorio) obliga a las páginas de GitHub a reconstruir su sitio con jekyll. El sitio reconstruido se puede ver unos segundos más tarde en <https://softwarebeasts.github.io>; si no, darle diez minutos como sugiere GitHub y aparecerá pronto.

> Existen tres formas diferentes en que puede realizar cambios en los archivos del blog:

> 1. Editando archivos dentro del nuevo repositorio softwarebeasts.github.io en el navegador en GitHub.com (se muestra a continuación).
> 2. Utilizando un editor de contenido de GitHub, como [Prose por Development Seed] (http://prose.io). Está optimizado para su uso con Jekyll, lo que hace la edición de marcado, la escritura de borradores y la carga de imágenes que sean realmente sencillas.
> 3. Clonando el repositorio y haciendo actualizaciones localmente, luego subiéndolo al repositorio de GitHub.

![_config.yml](/images/config.png "_config.yml")

### Paso 3) Publicar la primera entrada del blog

Editando `/_posts/2014-3-3-Hello-World.md` para publicar la primera entrada del blog.

![First Post](/images/first-post.png "First Post")

> ¡También se pueden agregar publicaciones adicionales en el navegador en GitHub.com! Simplemente se presiona el ícono + en `/ _posts /` para crear contenido nuevo. Solo hay que asegurarse de incluir el bloque [front-matter] (http://jekyllrb.com/docs/frontmatter/) en la parte superior de cada nueva publicación de blog y asegurarse de que el nombre del archivo de la publicación esté en este formato: año-mes-día-título.md

## Desarollo en local

1. Instalamos Jekyll y sus plugins de una sola vez. `gem install github-pages` Esto refleja los plugins utilizados por GitHub Pages en local, incluidos Jekyll, Sass, etc.
2. Clonamos nuestro repositorio con `git clone https://github.com/SoftwareBeasts/softwarebeasts.github.io.git`
3. Servimos el sitio y observamos los cambios del marcado/sass con `jekyll serve`
4. Vemos la página web en http://127.0.0.1:4000/
5. Hacemos commit de cualquier cambio y enviamos todo a la rama principal del repositorio de GitHub. GitHub Pages luego reconstruirá y servirá al sitio web.
