---
layout: post
title:  "Tutorial: Página web con Jekyll y GitHub Pages."
date:   2024-04-14 13:12:00 -0400
categories: tutorial
permalink: /:categories/:year/:month/:day/:title/
---

![octojekyll](/assets/images/octojekyll.png){:style="display:block; margin-left:auto; margin-right:auto; background-color:#333333"}

### Introducción.
[Jekyll](https://jekyllrb.com/) es una herramienta gratuita que nos permite la generación de web estáticas simples. Nos permite transformar documentos en texto plano a archivos HTML. Además, cuenta con capacidad de Blog. 

[GitHub Pages](https://pages.github.com/) Nos permite hostear una página web estática desde un repositorio público de nuestra cuenta de GitHub.

### Creación del repositorio.
Desde nuestra cuenta [GitHub](https://github.com/) crearemos un repositorio publico cuyo nombre tendrá la forma: **username.github.io**. Luego lo clonamos en nuestro equipo.

### Instalación de Jekyll.
Dependiendo del sistema operativo seleccionamos el que corresponde de la guía oficial de [instalación](https://jekyllrb.com/docs/installation/).

### Creación del proyecto.
Desde la carpeta de nuestro repositorio clonado ejecutamos el comando de terminal:
```console
jekyll new --skip-bundle .
```
Abrimos el archivo Gemfile y al principio de la línea que comienza con `gem "jekyll"` agregamos un `#` para comentarla.

Agregamos la *github-pages gem* creando una nueva línea en el archivo Gemfile con lo siguiente:<br />
`gem "github-pages", "~> GITHUB-PAGES-VERSION", group: :jekyll_plugins`.

Buscamos y reemplazamos **GITHUB-PAGES-VERSION** con la correspondiente [Dependency version]( https://pages.github.com/versions/). Guardamos los cambios del archivo Gemfile y ejecutamos:
```console
bundle install
```
Ejecutamos el servidor local:
```console
bundle exec jekyll serve
```
Ya podemos previsualizar nuestro sitio en el navegador: `http://localhost:4000`.<br />
En caso de error agregamos webrick e intentamos ejecutar el servidor nuevamente:
```console
bundle add webrick
```
### Agregar nuevos posts.
Los posts que vayamos creando los escribimos en formato [markdown]( https://es.wikipedia.org/wiki/Markdown) (archivos .md) y los guardamos en la carpeta `_posts`. Jekyll los convertirá automáticamente a HTML cada vez que ejecutemos el servidor local o cuando se suba al repositorio remoto.

El nombre de los archivos sigue el fomato: `año-mes-dia titulo_del_post.md` y el texto inicial del archivo debe contener los siguientes parámetros:<br />
```
---
layout: post
title: "Mi titulo."
date: 2024-04-14 13:12:00 -0400
categories: tutorial
---
```
Donde:<br />
`---`: Delimitador de los parametros para procesar el archivo.<br />
`layout`: post (plantilla para posts).<br />
`title`: Titulo de la publicación.<br />
`date`: Fecha de la publicación en formato año-mes-día.<br />
`categories`: Categoría de la publicación (se incluye en la url).<br />

### Publicación.
Para publicar nuestra web hacemos `commit` de nuestros cambios y los subimos al repositorio remoto mediante `push`, esperamos unos minutos y podremos ver nuestra web desde el navegador en la dirección: **username.github.io**.

Jekyll nos ofrece un amplio rango de opciones, así como temas para crear nuestra página. La [documentación](https://jekyllrb.com/docs/) oficial es la mejor forma para conocerlos y personalizar nuestra web.

