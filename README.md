# Favicons

## Good enough favicon

1. Go here https://realfavicongenerator.net/
2. generate favicons
3. put the following in the website root folder
  - favicon.ico
  - favicon-16x16.png
  - favicon-32x32.png
  - apple-touch-icon.png
4. add the following to <head> of index.html
  - <link rel="icon" href="favicon.ico" type="image/x-icon">
  - <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">

## Reference

css-tricks.com
https://css-tricks.com/favicon-quiz/

and the comment in the same post:

Federico Brigante
Permalink to comment# August 18, 2014

Unless you really really want your icons to be perfect and every size (and therefore you’re not simply using an automatic generator, which defeats the purpose) you only need two:

favicon.ico: 32×32 png file with .ico extension that looks decent at 16×16. You don’t even need to reference it in the html, browsers look for it automatically at the root, that is: http://www.example.com/favicon.ico
a 152×152 png file referenced as <link rel="apple-touch-icon" href="/icon.png">

There’s no need to clutter every and each request with that much code.
