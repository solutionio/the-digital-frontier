# README

This repo contains a collection of links and some thoughts on a development workflow & stack to build websites - not web applications. 

The theme structure should be universal. Either to use jekyll as a static page generator or wordpress as “backends”.

For the jekyll on github-pages usecase the development stack should have only basic requirements. Additional package managers and build tools like npm, bower, grunt or gulp should be optional. 

## TODO
- [x] create repository
- [x] add stuff from multiple projects to this repository
- [x] invite some nice people to collaborate
- [ ] create first iteration of the toolset


Gesetzt:

- jekyll
- wordpress
- magento

- npm
- bower
- gulp

- normalize
- bourbon
- neat / susy
- bitters
- refills
+ pesticide > http://pesticide.io/

- jquery

- - - - - - - - - - - - - - - - - - - - - - - - - - - - -

**workflow** ? 
hier festhalten wie eine workflow idealerweise aussieht

iteration 1
- workshop
- style tile (sketch)
- code
- release

iteration 2
- workshop
- style tile (sketch)
- code
- release

…


- - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

1. Was soll hier passieren?
> Eine kleine Linksammlung mit Interessantem Material zum bau von Webseiten > **Achtung** nicht Web Applikationen.
2. Umsetzung als Boilerplate / Workflow
> Standards für verschiedene Themen definieren.
- “Backend”: Jekyll und Wordpress
- Hosting: Welche Anbieter
- Deployment:
> Jekyll
> Wordpress
-  Front-End Architektur
> Styleguide zum schreiben von HTML / CSS (SASS) / JS
> Ordnerstruktur die für Jekyll / Wordpress Projekte gleichbleibt. 

Tools:
> npm
> bower
> gulp

SASS: 
- bourbon > nicht compass da jekyll projekte auf github pages das css bauen können sollten. dafür muss bourbon aber auch im sass folder liegen > nicht in bower_components
- neat


Standardelemente:
- Navigation (Off Canvas, Fullscreen, Text,…)
- Text
- Einzelbild (Inline, Lightbox)
- Bildergallerie (Inline, Lightbox)
- Masonry Grid
- Fullscreen Video (Inline, Lightbox)
- Fullscreen Image mit Text drauf
- Slider (Inline, Fullscreen)
- Google Maps Karte
- Sound / Audio Player

Use Cases:
- Landing Page
- Corporate Page
- Portfolio
- Shop 


**ALS BEISPIEL** - Was kann man besser machen?
<pre style=“max-height: 300px;”><code>Theme Root
    │    ├── assets
    │    │   ├── bower_components
    │    │   |   ├── bi-app-sass
    │    │   |   ├── bourbon
    │    │   |   └── neat
    │    │   ├── css
    |    |   |    ├── rtl-min.css
    |    |   |    ├── rtl.css
    |    |   |    ├── style-min.css
    |    |   |    └── style.css
    │    |   └──  js
    │    │   |    ├── app
    │    │   |    └── vendor
    │    |   |    |   ├── flexnav
    │    |   |    |   ├── hoverintent
    │    |   |    |   ├── modernizr
    │    |   |    |   └── selectivizr
    │    │   |    ├── production-min.js
    │    │   |    └── development.js
    │    ├── sass
    │    |   └── base (Bitters)
    │    |   └── components
    |    |    |   ├── _buttons.scss
    |    |    |   ├── _dashicons.scss
    |    |    |   ├── _flexnav.scss
    |    |    |   ├── _navigation.scss
    |    |    |   ├── _ui-bourbon.scss
    |    |    |   └── _variables.scss
    │    |    └── layouts
    |    |    |   ├── _content.scss
    |    |    |   ├── _footer.scss
    |    |    |   ├── _header.scss
    |    |    |   ├── _navigation.scss
    |    |    |   ├── _normalize.scss
    |    |    |   ├── _sidebar.scss
    |    |    |   ├── _structure.scss
    |    |    |   └── _typography.scss
    |    ├── _app.scss
    |    ├── _grid-settings.scss
    |    ├── _rtl.scss
    |    └── style.scss
    ├── library
    │   └── languages
    │   │   ├── some_like_it_neat.pot
    │   └── vendors
    │   │   ├── js
    │   │   ├── tgm-plugin-activation
    │   │   ├── tha-theme-hooks
    │   │   └── customizer
    │   ├── custom-header.php
    │   ├── extras.php
    │   ├── jetpack.php
    │   └── template-tags.php
    ├── page-templates
    │     └── partials
    |     |   ├── content-aside.php
    |     |   ├── content-audio.php
    |     |   ├── content-chat.php
    |     |   ├── content-gallery.php
    |     |   ├── content-image.php
    |     |   ├── content-link.php
    |     |   ├── content-none.php
    |     |   ├── content-page.php
    |     |   ├── content-quote.php
    |     |   ├── content-single.php
    |     |   ├── content-status.php
    |     |   ├── content-video.php
    |     |   └── content.php
    |     ├── template-full-width.php
    |     ├── template-left-col.php
    |     └── template-right-col.php
    ├── .bowerrc
    ├── 404.php
    ├── archive.php
    ├── comments.php
    ├── footer.php
    ├── functions.php
    ├── gulpfile.js
    ├── header.php
    ├── index.php
    ├── license.txt
    ├── package.json
    ├── page.php
    ├── README.md
    ├── rtl.css
    ├── search.png
    ├── searchform.php
    ├── sidebar.php
    ├── single.php
    └── style.css</code></pre>



**ansehen>** 
- https://github.com/google/web-starter-kit
- YEOMAN
- http://yeoman.io/generators/
- z.B. https://github.com/wesleytodd/YeoPress



## Hosting
- Jekyll
  + Github Pages
  + Google App Engine
  + FTP

- Wordpress
  + Uberspace

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

## Dependencies 
- sass
- bourbon
+ **jekyll** should be optional > used for first iteration 
+ bitters (optional) > is in gemfile right now
+ neat (optional) > is in gemfile right now
+ refills (optional) > is in gemfile right now
+ **wordpress** + **woocommerce**

To use install optional stuff > bitters / neat / refills please go into _sass
and use the following commands:

For bourbon
```bash
cd _sass
bourbon install
```


For bitters
```bash
cd _sass
bitters install
```


For neat
```bash
cd _sass
neat install
```

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - 


### JEKYLL
Für jekyll sollte folgendes gelten. Der User kann das Repo forken und sofort loslegen. Falls er das Repo auscheckt > “git clone” sollten nur minimale Abhängigkeiten vorhanden sein. 

Gute Beispiele hierfür:
- [http://www.jekyllnow.com/](http://www.jekyllnow.com/)
- [http://rohanchandra.github.io/project/type/](http://rohanchandra.github.io/project/type/)

- [https://github.com/mmistakes/skinny-bones-jekyll](https://github.com/mmistakes/skinny-bones-jekyll) - Theme auf Bourbon / Neat Basis 
- [https://github.com/jenmyers/jenmyers.net](https://github.com/jenmyers/jenmyers.net) - Works with bourbon and neat
- [https://github.com/jenmyers/jekyll-kickoff](https://github.com/jenmyers/jekyll-kickoff) - jekyll kickoff also by jen myers
- [https://blog.bolt.co/2013/12/12/building-the-bolt-blog.html](https://blog.bolt.co/2013/12/12/building-the-bolt-blog.html) - Bisschen was zum Bau eines Themes mit jekyll + bourbon

## JEKYLL RESOURCES

- [https://github.com/ixti/jekyll-assets](https://github.com/ixti/jekyll-assets) 
- [https://github.com/zachalbert/zachalbert.com](https://github.com/zachalbert/zachalbert.com) - fein, nicht barebones - gulp, bower
- [https://github.com/penibelst/jekyll-compress-html](https://github.com/penibelst/jekyll-compress-html) - html compress für jekyll
- [https://medium.com/design-open/becoming-a-jekyll-god-ef722e93f771](https://medium.com/design-open/becoming-a-jekyll-god-ef722e93f771) - seiten mit jekyll mit pagespeed 96 von 100 punkten
- [http://www.jekyllnow.com/](http://www.jekyllnow.com/)
- [http://www.smashingmagazine.com/2014/08/01/build-blog-jekyll-github-pages/](http://www.smashingmagazine.com/2014/08/01/build-blog-jekyll-github-pages/)
- [http://paulstamatiou.com/responsive-retina-blog-development-part-1/](http://paulstamatiou.com/responsive-retina-blog-development-part-1/)
- [http://paulstamatiou.com/responsive-retina-blog-development-part-2/](http://paulstamatiou.com/responsive-retina-blog-development-part-2/)
- [https://github.com/screeninteraction/jekyll-multiple-languages-plugin](https://github.com/screeninteraction/jekyll-multiple-languages-plugin) - multilingual sites with jekyll




### WORDPRESS BOILERPLATES
- [underscores.me](http://underscores.me)
- [https://github.com/Automattic/_s](https://github.com/Automattic/_s) [https://github.com/toddmotto/html5blank](https://github.com/toddmotto/html5blank)
- [https://github.com/digisavvy/some-like-it-neat](https://github.com/digisavvy/some-like-it-neat)
- [https://github.com/wp-cli/wp-cli](https://github.com/wp-cli/wp-cli)
- [https://github.com/roots/sage](https://github.com/roots/sage)
- [https://github.com/bigemployee/BigBlankTheme](https://github.com/bigemployee/BigBlankTheme)
- [https://github.com/murtaugh/HTML5-Reset-WordPress-Theme](https://github.com/murtaugh/HTML5-Reset-WordPress-Theme)


### WORDPRESS WOOCOMMERCE
- [https://github.com/woothemes/storefront](https://github.com/woothemes/storefront)
- [https://github.com/woothemes/boutique](https://github.com/woothemes/boutique) – Nils J. Nilsson 


### WORDPRESS - DEPLOYMENT STUFF
- [https://speakerdeck.com/chluehr/zero-to-hero-en](https://speakerdeck.com/chluehr/zero-to-hero-en) - ganz feiner Talk zu automatisiertem Deployment mit Ansible und Phing
- [https://roots.io/bedrock/](https://roots.io/bedrock/) – Wordpress deployment
- [https://github.com/markjaquith/WordPress-Skeleton](https://github.com/markjaquith/WordPress-Skeleton)
- [https://github.com/Mixd/wp-deploy](https://github.com/Mixd/wp-deploy)
- [http://code.tutsplus.com/articles/an-introduction-to-deploying-wordpress-with-mina--wp-34776](http://code.tutsplus.com/articles/an-introduction-to-deploying-wordpress-with-mina--wp-34776)
- [http://seravo.fi/2014/guide-to-modern-wordpress-deployment-part-1](http://seravo.fi/2014/guide-to-modern-wordpress-deployment-part-1)
- [http://seravo.fi/2014/guide-modern-wordpress-deployment-part-2](http://seravo.fi/2014/guide-modern-wordpress-deployment-part-2)
- []()


### WORDPRESS knowlege for local development

- Better Permalinks with MAMP on OSX
Change following config in /Applications/MAMP/conf/apache/

# Changed for Permalinks in Wordpress
# AllowOverride is normaly set to none
```bash
<Directory />
    Options Indexes FollowSymLinks
    AllowOverride All
</Directory>
```

This allows to have proper urls for WPML in local development


### WORDPRESS - PLUGINS
hier noch definiren was standard und was optional ist

#### STANDARD
- http://www.advancedcustomfields.com/
- http://wp-types.com/
- akismet
- bbpress
- buddypress
- backup buddy
- wpml	
- google xml sitemap
- jetpack
- wp-dbmanager
- google analytics dashboard
- contact form 7
- wp-piwik
- custom login > https://wordpress.org/plugins/custom-login/
- woocommerce
- wpseo 
- wordpress seo plugin von yoast
- w3 total cache
- wp super cache
- regenerate thumbnails
- iThemes Security
- Limit Login Attempts


#### OPTIONAL
- disqus comments
- facebook comments
- https://wordpress.org/plugins/seo-facebook-comments/
- https://wordpress.org/plugins/facebook-comments-plugin/







