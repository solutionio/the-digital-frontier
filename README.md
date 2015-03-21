# README

This repo contains a collection of links and some thoughts on a development workflow & stack to build websites - not web applications. 

The theme structure should be universal. Either to use jekyll as a static page generator or wordpress as “backends”.

For the jekyll on github-pages usecase the development stack should have only basic requirements. Additional package managers and build tools like npm, bower, grunt or gulp should be optional. 

- [http://12factor.net/](http://12factor.net/) - must read
- [http://archetyped.com/know/redesigning-archetyped-comparing-css-frameworks/](http://archetyped.com/know/redesigning-archetyped-comparing-css-frameworks/)- lightweight bourbon vs heavy foundation

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
either use the standard normalize or a scss version. the standard sass version of normalize isn’t working without compass. an older bower package for normalize is available and used right now. 
	* [https://github.com/JohnAlbin/normalize-scss](https://github.com/JohnAlbin/normalize-scss)
	* [https://github.com/krisbulman/normalize-libsass](https://github.com/krisbulman/normalize-libsass) - this one is for use with libsass > gulp-sass 
- bourbon
- neat / susy
- bitters
- refills > needs **neat** for some components
+ pesticide - a super nice dev tool
[http://pesticide.io](http://pesticide.io) - use it and love it!
	* maybe use it in combination with a “dev” parameter > or leave the switch for on/off > true/false in the main scss file. 

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
- [https://github.com/roots/sage](https://github.com/roots/sage) -  has a really need workflow, but it uses bootstrap atm.
	* [http://wptavern.com/roots-starter-theme-for-wordpress-will-become-framework-agnostic-in-2015](http://wptavern.com/roots-starter-theme-for-wordpress-will-become-framework-agnostic-in-2015) - **the roots theme will become framework agnostic in 2015 > might be a good starting point!**
	* [https://discourse.roots.io/](https://discourse.roots.io/) - talk about roots theme development
- [https://github.com/bigemployee/BigBlankTheme](https://github.com/bigemployee/BigBlankTheme)
- [https://github.com/murtaugh/HTML5-Reset-WordPress-Theme](https://github.com/murtaugh/HTML5-Reset-WordPress-Theme)
- [https://github.com/synapticism/wordpress-gulp-bower-sass](https://github.com/synapticism/wordpress-gulp-bower-sass) - another wordpress boilerplate using gulp, bower and sass
	* [http://synapticism.com/dev/wordpress-theme-development-with-gulp-bower-and-sass/](http://synapticism.com/dev/wordpress-theme-development-with-gulp-bower-and-sass/) - something to read about this boilerplate
- [https://github.com/zach-adams/cutlass-wp-theme](https://github.com/zach-adams/cutlass-wp-theme) - maybe to much > using different template engine
- [https://github.com/bueltge/WordPress-Basis-Theme](https://github.com/bueltge/WordPress-Basis-Theme) - altbekannt
- [https://github.com/bueltge/wordpress-basis-theme-Child-Starter](https://github.com/bueltge/wordpress-basis-theme-Child-Starter) - und das child theme dazu

### WORDPRESS KNOWLEGE / READING LIST
- [https://css-tricks.com/taking-control-cssjs-wordpress-plugins-load/](https://css-tricks.com/taking-control-cssjs-wordpress-plugins-load/)

### WORDPRESS CHEAT SHEETS
- [http://www.buildyourownblog.net/blog/time-saving-copypaste-wordpress-cheat-sheet/](http://www.buildyourownblog.net/blog/time-saving-copypaste-wordpress-cheat-sheet/)


### WORDPRESS WOOCOMMERCE
- [https://github.com/woothemes/storefront](https://github.com/woothemes/storefront)
- [https://github.com/woothemes/boutique](https://github.com/woothemes/boutique) – Nils J. Nilsson 

### WORDPRESS CHILD THEME
- [http://code.tutsplus.com/tutorials/how-to-modify-the-parent-theme-behavior-within-the-child-theme--wp-31006](http://code.tutsplus.com/tutorials/how-to-modify-the-parent-theme-behavior-within-the-child-theme--wp-31006) - Child Theme Erstellung > Parent Theme Features sauber entfernen. 

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
- google xml sitemap
- jetpack
- wp-dbmanager
- google analytics dashboard
- contact form 7
- wp-piwik
- custom login > https://wordpress.org/plugins/custom-login/
- wpseo 
- wordpress seo plugin von yoast
- w3 total cache
- wp super cache
- [https://wordpress.org/plugins/cachify/](https://wordpress.org/plugins/cachify/) - einfacher zu konfigurieren
- regenerate thumbnails
- iThemes Security
- Limit Login Attempts


#### MULTILINGUAL
- WPML Multilingual CMS
- WPML String Translation
- WPML Translation Management
- WPML Media

- [https://wordpress.org/plugins/woocommerce-multilingual/](https://wordpress.org/plugins/woocommerce-multilingual/)

#### STORE
- WooCommerce

#### STORE MULTILINGUAL
- WooCommerce Multilingual (for usage with WPML)
- WooCommerce Germanized (kostenlos)
https://vendidero.de/dokument/woocommerce-germanized-theme-kompatibilitaet
- WooCommerce German Market

http://wpml.org/de/documentation-3/ahnliche-projekte/woocommerce-multilingual-betreiben-sie-e-commerce-seiten-in-mehreren-sprachen/

- [http://wpml.org/documentation/theme-compatibility/storefront-wpml-create-a-multilingual-shop/](http://wpml.org/documentation/theme-compatibility/storefront-wpml-create-a-multilingual-shop/) - create a multilingual shop with storefront & wpml

#### STORE PLUGINS
- Rechnungen
- Lieferscheine
- Versandlabel > DHL?
- Video
- [https://marketpress.de/2014/woocommerce-rechnung-lieferschein/?noredirect=de_DE](https://marketpress.de/2014/woocommerce-rechnung-lieferschein/?noredirect=de_DE)

- [http://codecanyon.net/item/shipping-details-plugin-for-woocommerce/2018867](http://codecanyon.net/item/shipping-details-plugin-for-woocommerce/2018867)
- [http://www.woothemes.com/products/print-invoices-packing-lists/](http://codecanyon.net/item/shipping-details-plugin-for-woocommerce/2018867 )




#### OPTIONAL
- disqus comments
- facebook comments
- https://wordpress.org/plugins/seo-facebook-comments/
- https://wordpress.org/plugins/facebook-comments-plugin/
- [https://wordpress.org/plugins/toolbox/](https://wordpress.org/plugins/toolbox/) - funktionen als module auslagern

## DOCUMENTATION
Will happen in this repository. A good guide about using markdown on github:
- [https://guides.github.com/features/mastering-markdown](https://guides.github.com/features/mastering-markdown)
- Either use iA Writer, Sublime, Atom or a webbased tool like [http://prose.io/](http://prose.io/) to edit markdown files.


## DEV WORKFLOW FOR SASS
use gulp with livereload, browsersync, sass sourcemaps to work in chrome dev tools 
- [https://github.com/dlmanning/gulp-sass](https://github.com/dlmanning/gulp-sass) - gulp sass speeds up the whole thing - using libsass instead of ruby sass…
- [https://developer.chrome.com/devtools/docs/workspaces](https://developer.chrome.com/devtools/docs/workspaces) - chrome dev tools workspaces
- [https://medium.com/@toolmantim/getting-started-with-css-sourcemaps-and-in-browser-sass-editing-b4daab987fb0](https://medium.com/@toolmantim/getting-started-with-css-sourcemaps-and-in-browser-sass-editing-b4daab987fb0)
- [http://www.sitepoint.com/using-source-maps-debug-sass-chrome/](http://www.sitepoint.com/using-source-maps-debug-sass-chrome/) - how to do source maps
- [https://chrome.google.com/webstore/detail/devtools-theme-zero-dark/bomhdjeadceaggdgfoefmpeafkjhegbo](https://chrome.google.com/webstore/detail/devtools-theme-zero-dark/bomhdjeadceaggdgfoefmpeafkjhegbo) - dark theme for chrome dev tools


## UNCSS
- [http://addyosmani.com/blog/removing-unused-css/](http://addyosmani.com/blog/removing-unused-css/) - find and remove unused CSS
- [https://github.com/giakki/uncss](https://github.com/giakki/uncss)
- [https://github.com/ben-eb/gulp-uncss](https://github.com/ben-eb/gulp-uncss)

## Meta Tags
- [https://gist.github.com/kevinSuttle/1997924](https://gist.github.com/kevinSuttle/1997924)
- [http://davidwalsh.name/facebook-meta-tags](http://davidwalsh.name/facebook-meta-tags)
- [http://www.quicksprout.com/2013/03/25/social-media-meta-tags-how-to-use-open-graph-and-cards/](http://www.quicksprout.com/2013/03/25/social-media-meta-tags-how-to-use-open-graph-and-cards/)




