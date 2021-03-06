# Jekyll Blog 1 Column Example (Gulp) · [Demo](http://bcasal.github.io/Jekyll-Blog_1Column-Example/)

Blog creado con [**Jekyll**](https://jekyllrb.com/) a partir de la estructura básica
que genera por defecto el comando `$ jekyll new .` con algunos complementos,
modificaciones y personalizaciones.
**Jekyll** (
  [Docs](https://jekyllrb.com/docs/home/),
  [GitHub](https://github.com/jekyll/jekyll),
  [WebSite](https://jekyllrb.com/),
  [Twitter](https://twitter.com/jekyllrb),
  [License](https://github.com/jekyll/jekyll/blob/master/LICENSE)
  )

Listo para utilizar con
[GitHub-Pages!!!](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/)

```
// clone
$ git clone https://github.com/BCasal/Jekyll-Blog_1Column-Example.git

// rename
$ mv Jekyll-Blog_1Column-Example New-FolderName
$ cd New-FolderName

// install dep.
$ sudo gem install jekyll-paginate
$ npm install

// config
$ nano _config.yml

// run
$ gulp
```

## Tareas Gulp

El comando `$ gulp` ejecuta dos tareas "Jekyll" y "Serve".

* Jekyll, ejecuta las mismas tareas que si se ejecutara el comando `jekyll serve`
  en un proyecto Jekyll por defecto, excepto, montar el servidor local.
* Serve, se encarga de montar el servidor local con BrowserSync
  en la carpeta `_site`
  
Hay una tarea llamada "Sass" que procesa los archivos CSS ya compilados,
añadiendo los prefijos necesarios y minificando el archivo.

> WARNING!!! Algunas veces, la primera vez que arranca browser-sync no muestra
> correctamente la página, para visualizar la página hay que refrescar el
> navegador manualmente, et voilà !

## Complementos

### Plugin de busqueda **Simple Jekyll Search** by ***Christian Fei***.

Plugin (
  [Simple Jekyll Search](https://github.com/christian-fei/Simple-Jekyll-Search),
  [How to use](https://github.com/christian-fei/Simple-Jekyll-Search/blob/master/README.md),
  [License](https://github.com/christian-fei/Simple-Jekyll-Search/blob/master/LICENSE.md)
  )

Author (
  [WebSite](http://christian.fei.ninja/),
  [GitHub](https://github.com/christian-fei),
  [Twitter](https://twitter.com/christian_fei)
  )

### Plugin de paginación **Jekyll Paginate** para el listado de Posts.

Plugin (
  [Jekyll Paginate](https://github.com/jekyll/jekyll-paginate),
  [How to use](https://jekyllrb.com/docs/pagination/),
  [License](https://github.com/jekyll/jekyll-paginate/blob/master/LICENSE.txt)
  )

### Font Awesome Icon Font

Icon Font (
  [WebSite](http://fontawesome.io/),
  [How to use](https://fortawesome.github.io/Font-Awesome/examples/),
  [GitHub](https://github.com/FortAwesome/Font-Awesome/),
  [Twitter](https://twitter.com/fontawesome),
  [License](https://fortawesome.github.io/Font-Awesome/license/)
  )

## Imágenes

Backgrounds (
  [Cabecera](https://openclipart.org/detail/221300/abstract-polygon-background),
  [Footer](http://wallpaperswide.com/polygon_green-wallpapers.html)
  )
