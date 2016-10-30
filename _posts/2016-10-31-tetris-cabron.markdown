---
layout: post
title:  "El Tetris cabrón"
date:   2016-10-31 10:10:06
categories: juegos
tags: bastet, tetris
image: /assets/article_images/2016-10-31-tetris-cabron/bastet-header.png
---
Muchos lo conocerán ya desde hace tiempo, pero me apetecía rememorar este juego libre de consola que a más de uno le traerá dolores de cabeza cuando lo pruebe.

Se trata de **Bastard Tetris** (bastet para los amigos), otro juego clónico del clásico Tetris, programado con ncurses que apenas difiere de la mecánica del juego original, pero con la peculiaridad de ser un tetris bastante cabrón.

![](/assets/article_images/2016-10-28-tetris-cabron/bastet-ss1.png) 

Cabrón porque está programado intencionadamente para ponerle las cosas difíciles al jugador, pues tiene un algoritmo que calculará milimétricamente cada pieza que coloques en el juego para luego sacarte la peor pieza posible en el siguiente turno. Es decir, ni se te ocurra en este juego intentar formar un gran cañón para completar varias líneas de golpe con la pieza 'I' porque el juego hará que eso sea imposible.

Hay dos modalidades de juego: normal y difícil. En la primera puedes ver al menos cuál será la pieza que saldrá a continuación del turno actual y se calculará la peor pieza a partir del segundo turno, mientras que en el modo difícil se complica más la cosa ya que ni se mostrará cuál será la siguiente pieza, y se aprovecha de esa característica para que desde el primer turno, el juego vaya sacando siempre la peor pieza posible.

El autor del juego, Federico Poloni, lo describe como _"una alternativa atractiva a Microsoft Word dedicada a aquellos usuarios que disfrutan insultando a su ordenador"_.

Puedes encontrar su código fuente con sus instrucciones de compilación e instalación en su repositorio de [GitHub](https://github.com/fph/bastet/). Se puede instalar en sistemas Unix y GNU/Linux, aunque también se han realizado ports para Windows. Se encuentra también disponible en numerosos gestores de paquetes:

* Arch Linux y derivados (Manjaro, Antergos, Apricity, etc).
{% highlight sh %}
pacman -S bastet
{% endhighlight %}
* Debian y derivados (Ubuntu, Mint, etc).
{% highlight sh %}
apt-get install bastet
{% endhighlight %}
* Fedora / RHEL y derivados (Korora, Viperr, etc).
{% highlight sh %}
yum install bastet
{% endhighlight %}
* Gentoo y derivados (Funtoo, Sabayon, etc).
{% highlight sh %}
emerge games-puzzle/bastet
{% endhighlight %}
* FreeBSD.
{% highlight sh %}
pkg install bastet
{% endhighlight %}
