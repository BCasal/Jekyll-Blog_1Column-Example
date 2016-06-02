---
layout: 	    post

title: 		    "Code Snippets"
date: 		    2016-05-19 19:24
author: 	    "Code"
categories:   [Jekyll, Blog]
tags: 		    [Posts, Tips, Code]
icon: 		    "code"

excerpt: >
  Si quieres añadir una entradilla personalizada para
  mostrar en el listado de los posts, añadela en la
  cabecera YFM `excerpt: bla bla bla`, esta misma
  entradilla se utiliza para completar la etiqueta
  `meta name="description"` de la página generada
  para el post.
---

### Block Code

Crear bloques de código:

```
  ```
    def print_hi(name)
      puts "Hi, #{name}"
    end
    print_hi('Tom')
    #=> prints 'Hi, Tom' to STDOUT.
  ```
```

### Syntax Highlighting

Añadiendo el lenguaje del bloque de código se activa el
Syntax Highlighting.

```
  ``` ruby
    def print_hi(name)
      puts "Hi, #{name}"
    end
    print_hi('Tom')
    #=> prints 'Hi, Tom' to STDOUT.
  ```
```

et voilà !

``` ruby
  def print_hi(name)
    puts "Hi, #{name}"
  end
  print_hi('Tom')
  #=> prints 'Hi, Tom' to STDOUT.
```
