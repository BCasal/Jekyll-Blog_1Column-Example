---
layout: 	    post

title: 		    "Links Alias (Markdown Tips)"
date: 		    2016-05-19 19:26
author: 	    "Links"
categories:   [Jekyll, Blog]
tags: 		    [Posts, Tips, Markdown]
icon: 		    "link"

excerpt: >
  Utilizando **Alias** para los enlaces, mantienes
  una lectura clara de los posts mientras los escribes.
---

### Links (Alias)

Para mantener una lectura clara de los posts, evita hacer esto
con los enlaces.

``` markdown
  Check out the [Jekyll docs](http://jekyllrb.com/docs/home) for more info.
  Bugs/feature requests at [Jekyll’s GitHub repo](https://github.com/jekyll/jekyll).
  If you have questions, you can ask them on [Jekyll Talk](https://talk.jekyllrb.com/).
```

Es mejor crear una lista de Alias al final del post como esta.

``` markdown
  [jekyll-docs]: http://jekyllrb.com/docs/home
  [jekyll-gh]:   https://github.com/jekyll/jekyll
  [jekyll-talk]: https://talk.jekyllrb.com/
```

Y utilizarla asi.

``` markdown
Check out the [Jekyll docs][jekyll-docs] for more info.
Bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh].
If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].
```

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
