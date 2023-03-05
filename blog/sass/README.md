# From minima jekyll theme

Work on scss to make a personal css file on my website : <https://web.lunarviews.net>

&nbsp;

## Get minima info  

```bash
❯ gem info minima

*** LOCAL GEMS ***

minima (2.5.1)
    Author: Joel Glovier
    Homepage: https://github.com/jekyll/minima
    License: MIT
    Installed at: /usr/lib/ruby/gems/3.0.0

    A beautiful, minimal theme for Jekyll.

```

&nbsp;

## Compilation from compile-sass.dart

Clone repo:

```bash
git clone https://github.com/rnek0/helloWorldSass
```

Compile :

```bash
dart compile-sass.dart /home/rnek0/codes/WEB/CSS/sass/helloWorldSass/blog/sass/minima.scss /home/rnek0/codes/WEB/CSS/sass/helloWorldSass/blog/sass/main.css

sleep 1

less /home/rnek0/codes/WEB/CSS/sass/helloWorldSass/blog/sass/main.css

```

