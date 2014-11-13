


Ghost-theme  
======

fork from https://github.com/mholland1337/Mutiny

A free premium bootstrap Ghost theme
 Mutiny is a clean, minimal Ghost theme with all the bells and whistles.

Built in [Boostrap 3](http://getbootstrap.com/) Mutiny is can be easily customized to meet your needs. You can add your own custom bootstrap theme to overwite the default boostrap stylesheet. Mutiny currently comes with the [bootswatch](http://bootswatch.com/) theme [cosmo](http://bootswatch.com/cosmo/) as default.

## Features
* Built in Boostrap 3
* Easily customizable
* Infinite scroll
* Custom tags page
* Google authorship
* Responsive design
* Image lightbox
* Disqus comment support
* [Structured data](http://www.google.com/webmasters/tools/richsnippets?q=maxholland.me)

## Installation
1. Download the theme 
2. Extract the .zip file.
3. Make the appropriate changes e.g. side bar links
4. Re-zip the file and upload to your ghost blog.

## Changing the boostrap theme
1. Go into the partials folder.
2. Open up **bootstrap-theme.hbs** in your text editor.
3. Replace the stylesheet link with your link.
4. You can find some great themes from [bootswatch here](http://www.bootstrapcdn.com/#bootswatch_tab)

Original:
`<link rel="stylesheet" type="text/css" href="{{asset "css/cosmo-theme.css"}}" />`

Changed :
`<link rel="stylesheet" type="text/css" href="//maxcdn.bootstrapcdn.com/bootswatch/3.2.0/slate/bootstrap.min.css" />`


## Changing navbar links
1. Go into the partials folder.
2. Open up **navbar.hbs** in your text editor.
3. Replace the existing link **href** with your link.

## Adding navbar links
1. Go into the partials folder.
2. Open up **navbar.hbs** in your text editor.
3. Copy and paste the <li> tag and change it to be your link e.g.

Original:
`<li><a href="/about">About</a></li>`

New Link:
`<li><a href="/Hello">Hello</a></li>`

## Changing social links
1. Go into the partials folder.
2. Open up **footer.hbs** in your text editor.
3. Replace the existing link **href** with your link.

#### Adding a new social link.
1. Follow steps 1. & 2. above.
2. Copy one the the lines of code under the links heading.
3. Change the href to be your link and the text to be your text.


## Adding Disqus comments
1. Go into the partials folder.
2. Open up **comments.hbs**.
3. Replace the disqus shortname with your disqus shortname (see example)
4. Save it.
5. Open up **post.hbs**.
6. Un-rem the comment code. Example below

Remmed out:
`<!--{{> comments}}-->`

Un remmed:
`{{> comments}}`

## GooglePlus Authorship
1. Go into the partials folder.
2. Open up **google-authorship.hbs**.
3. Paste the link of your google plus profile into href="" (see example)