---
layout: post
title: "GitHub (Pages) y Jekyll: Vivisección"
---

{{ page.title }}
================

<p class="meta">July 21 2011</p>

Como mencioné en [mi primer post](http://fireblend.github.com/2011/07/19/a-new-blog.html), algunas veces este blog contará con contenido en inglés y otras en español. ¿Por qué? Porque (como también mencione) creo que muchas veces hablar acerca de un tema en particular en inglés es recorrer camino ya muy bien explorado en ese idioma mientras que encontrar recursos acerca del mismo en español es un reto. 

No que dentro del contexto tecnológico en el que el contenido de este blog se desarrolla el conocimiento del inglés no sea una necesidad y obligación básica para quien quiera obtener la más mínima cantidad de información no solo directo de su fuente (con sus notables excepciones), sino también a tiempo para asegurarse el contar con una base actualizada de conocimiento en el área.

En fín, este post trata acerca de la plataforma detrás de este blog. Como mencioné y es evidente, el blog existe como un repositorio en [GitHub](https://github.com/) y es publicado por medio de su servicio de [GitHub Pages](http://pages.github.com/), como una página estática automáticamente generada por [Jekyll](http://jekyllrb.com/) y construida por GitHub cada vez que se aplica un cambio al repositorio. Vamos por partes.

[GitHub](https://github.com/) es un servicio de alojamiento para proyectos de desarrollo de software que usan el sistema de control de revisiones Git. Esta escrito en Ruby on Rails y Erlang, y actualmente cuenta con más de 2 millones de repositorios, la mayoría públicos (con una cuenta gratuita este es el único tipo de repositorios que se pueden crear), albergando proyectos de software libre. Su frase "Social Coding" es adecuada, no solo los proyectos tienen su sistema usual de manejo de peticiones y problemas por parte de usuarios, si no que el servicio posee su propio botón de "follow" al estilo de redes sociales para seguir el progreso de proyectos y programadores que sean de interes.

GitHub además ofrece el servicio de [GitHub Pages](http://pages.github.com/); al crear un repositorio llamado <usuario>.github.com  (como el que pueden ver en [mi cuenta en github](http://github.com/fireblend)) con un archivo index.html en su raiz, sus contenidos son publicados automáticamente en dicha dirección. En adición a esto, es posible crear páginas para proyectos (repositorios) con relativa facilidad, utilizando un generador automático integrado en el sitio.

[Jekyll](http://jekyllrb.com/) es el último de los ingredientes responsables de la creación de esta página. Este es un generador de sitios web estáticos con ciertas consideraciones para blogs; su aversión a páginas dinámicas y implementaciones complejas se refleja en lo minimalista que puede verse e internamente ser (aunque es enormemente extendible). Coincidentemente, Jekyll fue escrito por Tom Preston-Werner, uno de los creadores de GitHub, y es un proyecto de software libre con [su propio repositorio en el servicio](https://github.com/mojombo/jekyll/).

Crear un sitio web o blog con Jekyll [es simple](https://github.com/mojombo/jekyll/wiki/Usage), y realmente no necesita mucho conocimiento previo además de HTML y CSS básico. Basta con dar un vistazo al [código fuente de este sitio](https://github.com/Fireblend/fireblend.github.com) para darse cuenta de ello; no requiere de más que un par de "layout" files (archivos que utilizan la sintaxis de marcado [Liquid](http://www.liquidmarkup.org/) que definen la distribución de elementos para dados tipos de páginas, como "default" para la página de entrada y "posts" para páginas como esta que albergan posts del blog) y archivos .html comunes para la definición de sus contenidos. Los posts en sí no son más que archivos .md (Markdown) que soportan los sintaxis de marcado simple editables desde cualquier editor de texto Markdown y Textile, y cualquier modificación visual es facilmente realizada por medio de archivos CSS; muchas de las modificaciones de este sitio no son mas que juegos de CSS3 y HTML5.

Finalmente, el sitio puede ser construido localmente después de que Jekyll haya sido instalado ([un proceso simple](https://github.com/mojombo/jekyll/wiki/Install)) para ser probado antes de su publicación, y basta con un comando de git push para que este se publique sin problemas a GitHub Pages o el servicio que se desee de manera instantanea.

Esta ha sido solo una pequeña introducción a GitHub, su servicio de Pages y Jekyll, temas que puede que revisite eventualmente, en especial cuando me refiera a sistemas de control de revisiones y servicios como este, BitBucket y otros con fines similares, un tema del que también quiero poder hablar. Espero que haya sido de utilidad, y los invito a seguir leyendo el blog conforme agrego más contenido, buscando que este sea nuevo, y no como dije, exploraciones de terreno ya muy conocido.
