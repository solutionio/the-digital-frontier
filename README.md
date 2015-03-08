# README
THIS IS STILL A BIG MESS ;)

Gesetz:

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




### JEKYLL
- [https://github.com/screeninteraction/jekyll-multiple-languages-plugin](https://github.com/screeninteraction/jekyll-multiple-languages-plugin) - multilingual sites with jekyll


### BOURBON & JEKYLL


### BOURBON & WORDPRESS
- [https://github.com/digisavvy/some-like-it-neat](https://github.com/digisavvy/some-like-it-neat) – Nils J. Nilsson

### Wordpress Store Theme
- [https://github.com/woothemes/storefront](https://github.com/woothemes/storefront) – Nils J. Nilsson
- [https://github.com/woothemes/boutique](https://github.com/woothemes/boutique) – Nils J. Nilsson 


### WORDPRESS
- [underscores.me](http://underscores.me) – Nils J. Nilsson
- [https://github.com/Automattic/_s](https://github.com/Automattic/_s) – Nils J. Nilsson
- [https://github.com/toddmotto/html5blank](https://github.com/toddmotto/html5blank) – Nils J. Nilsson
- [https://github.com/wp-cli/wp-cli](https://github.com/wp-cli/wp-cli) – Nils J. Nilsson
- [https://github.com/roots/sage](https://github.com/roots/sage) – Nils J. Nilsson
- [https://github.com/bigemployee/BigBlankTheme](https://github.com/bigemployee/BigBlankTheme) – Nils J. Nilsson
- [https://github.com/murtaugh/HTML5-Reset-WordPress-Theme](https://github.com/murtaugh/HTML5-Reset-WordPress-Theme) –


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
<Directory />
    Options Indexes FollowSymLinks
    AllowOverride All
</Directory>

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





- [https://github.com/screeninteraction/jekyll-multiple-languages-plugin](https://github.com/screeninteraction/jekyll-multiple-languages-plugin)


- [http://cssguidelin.es/](http://cssguidelin.es/)
- [https://github.com/jenmyers/jenmyers.net](https://github.com/jenmyers/jenmyers.net)
- [https://github.com/google/web-starter-kit](https://github.com/google/web-starter-kit)
- [http://www.basscss.com/](http://www.basscss.com/)
- [https://github.com/jenmyers/jekyll-kickoff](https://github.com/jenmyers/jekyll-kickoff)
- [https://mmistakes.github.io/skinny-bones-jekyll/getting-started/](https://mmistakes.github.io/skinny-bones-jekyll/getting-started/)
- [https://github.com/rohanchandra/type-theme](https://github.com/rohanchandra/type-theme)
- [http://codyhouse.co/gem/alternate-fixed-scroll-backgrounds/](http://codyhouse.co/gem/alternate-fixed-scroll-backgrounds/)
- [http://mediaelementjs.com/](http://mediaelementjs.com/)
- [https://github.com/bensmithett/style](https://github.com/bensmithett/style)
- [https://speakerdeck.com/csswizardry/ten-principles-for-effective-front-end-development](https://speakerdeck.com/csswizardry/ten-principles-for-effective-front-end-development)


# TYPOGRAPHY
## Found this lately: http://typeplate.com/
Then following this articles from this [discussion] [1] :
*  [1]: https://github.com/typeplate/typeplate.github.com/issues/64
* http://informationarchitects.net/blog/responsive-typography-the-basics
* http://trentwalton.com/2012/06/19/fluid-type/

## I am still looking for a best practise
- [http://css-tricks.com/snippets/css/less-mixin-for-rem-font-sizing/](http://css-tricks.com/snippets/css/less-mixin-for-rem-font-sizing/)
- [https://github.com/ry5n/rem](https://github.com/ry5n/rem)
- [https://github.com/bitmanic/rem](https://github.com/bitmanic/rem)
- [http://gregrickaby.com/2013/02/golden-ratio-typography-for-sass.html](http://gregrickaby.com/2013/02/golden-ratio-typography-for-sass.html)

- [https://github.com/corysimmons/typographic](https://github.com/corysimmons/typographic)
- [http://jasonsantamaria.com/articles/baseline-grids-on-the-web](http://jasonsantamaria.com/articles/baseline-grids-on-the-web)
- [http://sassline.com/](http://sassline.com/)



## JS
- [https://muut.com/riotjs/](https://muut.com/riotjs/)


## BOILERPLATES
- [https://github.com/corysimmons/boy](https://github.com/corysimmons/boy)
- [http://sass.fffunction.co/](http://sass.fffunction.co/)


## FRAMEWORKS
- [http://spacebase.space150.com/](http://spacebase.space150.com/)
- [http://concisecss.com/](http://concisecss.com/)



## GRIDS
- [http://susy.oddbird.net](http://susy.oddbird.net)
- [https://github.com/ericam/susy/](https://github.com/ericam/susy/)
- [http://jeet.gs/](http://jeet.gs/)
- [https://github.com/mojotech/jeet](https://github.com/mojotech/jeet)
- [http://gridle.org/](http://gridle.org/)
- [https://github.com/olivierbossel/gridle](https://github.com/olivierbossel/gridle)
- [http://neat.bourbon.io/](http://neat.bourbon.io/)
- [https://github.com/thoughtbot/neat](https://github.com/thoughtbot/neat)
- [http://singularity.gs/](http://singularity.gs/)
- [https://github.com/at-import/Singularity](https://github.com/at-import/Singularity)
- [https://github.com/at-import/Singularity-extras](https://github.com/at-import/Singularity-extras)



- [https://github.com/thoughtbot/design-sprint](https://github.com/thoughtbot/design-sprint)





# RESOURCES

> I want to collect some interessting links to extract course materials from. As KHB (Berlin Academy of the Arts) really needs somebody teaching designers the basics of CSS / HTML.

## GENERAL

- [https://github.com/AllThingsSmitty/must-watch-css](https://github.com/AllThingsSmitty/must-watch-css)

- [http://sebastien-gabriel.com/designers-guide-to-dpi/](http://sebastien-gabriel.com/designers-guide-to-dpi/)
- [http://webfieldmanual.com/](http://webfieldmanual.com/)
- [http://www.staticapps.org/](http://www.staticapps.org/)
- [http://www.fizerkhan.com/blog/posts/Free-Static-Page-Hosting-on-Google-App-Engine-in-a-5-minutes.html](http://www.fizerkhan.com/blog/posts/Free-Static-Page-Hosting-on-Google-App-Engine-in-a-5-minutes.html)
- [https://github.com/blainegarrett/gae-static](https://github.com/blainegarrett/gae-static)
- [http://blog.superfeedr.com/asset-hosting-ssl-domain/](http://blog.superfeedr.com/asset-hosting-ssl-domain/)
- [https://github.com/fizerkhan/gae-static-pages](https://github.com/fizerkhan/gae-static-pages)
- [http://blog.freundorfer.at/2014/01/jekyll-on-app-engine-with-beautiful-urls/](http://blog.freundorfer.at/2014/01/jekyll-on-app-engine-with-beautiful-urls/)

## HIDE URL BAR

- [http://tech.pro/blog/1557/7-useful-mobile-html-css-and-javascript-snippets](http://tech.pro/blog/1557/7-useful-mobile-html-css-and-javascript-snippets)
- [http://www.html5rocks.com/en/mobile/fullscreen/](http://www.html5rocks.com/en/mobile/fullscreen/)
- [http://davidwalsh.name/hide-address-bar](http://davidwalsh.name/hide-address-bar)
- [https://github.com/h5bp/mobile-boilerplate/blob/master/js/helper.js](https://github.com/h5bp/mobile-boilerplate/blob/master/js/helper.js)
- [http://24ways.org/2011/raising-the-bar-on-mobile/](http://24ways.org/2011/raising-the-bar-on-mobile/)
- [https://github.com/scottjehl/Hide-Address-Bar](https://github.com/scottjehl/Hide-Address-Bar)
- [http://www.mobilexweb.com/blog/ios-7-1-safari-minimal-ui-bugs](http://www.mobilexweb.com/blog/ios-7-1-safari-minimal-ui-bugs)

> Geht im Grunde nur auf iOS6 mit JS (dort orientationchange beachten) > Interessant für iPhone 4 User. Auf Android Chrome gibt es wohl keine Lösung. Windows Mobile? Kerstin meinte da gibts was. iOS7 mit minimal UI Tag.


## MOBILE FIRST
- [http://www.abookapart.com/products/mobile-first](http://www.abookapart.com/products/mobile-first)


## OFFLINE FIRST

- [https://github.com/pazguille/offline-first](https://github.com/pazguille/offline-first)
- [http://www.sitepoint.com/offline-first-next-progressive-enhancement-technique/](http://www.sitepoint.com/offline-first-next-progressive-enhancement-technique/)
- [http://alistapart.com/article/offline-first](http://alistapart.com/article/offline-first)
- [http://5by5.tv/webahead/78](http://5by5.tv/webahead/78)
- [https://github.com/jakearchibald/tweetdeck-prototype](https://github.com/jakearchibald/tweetdeck-prototype)
- [http://blog.hood.ie/2013/11/say-hello-to-offline-first/](http://blog.hood.ie/2013/11/say-hello-to-offline-first/)
- [http://www.lukew.com/ff/entry.asp?1902](http://www.lukew.com/ff/entry.asp?1902)


## LOGIN / PASSWORD

- [https://passwordless.net/](https://passwordless.net/)
- [https://medium.com/@ninjudd/passwords-are-obsolete-9ed56d483eb](https://medium.com/@ninjudd/passwords-are-obsolete-9ed56d483eb)


## DJANGO

- [https://github.com/moccu/django-omnibus](https://github.com/moccu/django-omnibus)


## DJANGO + ANGULAR

- [http://blog.nknj.me/token-authentication-django-and-angular](http://blog.nknj.me/token-authentication-django-and-angular)
- [http://netengine.com.au/blog/gulp-and-angularjs-a-love-story-or-the-old-wheel-was-terrible-check-out-my-new-wheel/](http://netengine.com.au/blog/gulp-and-angularjs-a-love-story-or-the-old-wheel-was-terrible-check-out-my-new-wheel/)
- [http://blog.kevinastone.com/getting-started-with-django-rest-framework-and-angularjs.html](http://blog.kevinastone.com/getting-started-with-django-rest-framework-and-angularjs.html)



## SASS RESOURCES

- [http://thesassway.com/](http://thesassway.com/)
- [http://www.sache.in/](http://www.sache.in/)

## SASS "FRAMEWORKS"
- [http://concisecss.com/](http://concisecss.com/)
- [http://pointnorth.io/](http://pointnorth.io/)
- [http://bourbon.io/](http://bourbon.io/)
- [http://bitters.bourbon.io/](http://bitters.bourbon.io/)

## Johannes learning SASS (some notes)

* @extend
* @include
* %placeholder
* $variable
* @mixin

## FLEXBOX

- [http://philipwalton.github.io/solved-by-flexbox/](http://philipwalton.github.io/solved-by-flexbox/)
- [http://www.sketchingwithcss.com/samplechapter/cheatsheet.html](http://www.sketchingwithcss.com/samplechapter/cheatsheet.html)
- [http://heydesigner.com/flexbox/](http://heydesigner.com/flexbox/)
- [http://bennettfeely.com/flexplorer/](http://bennettfeely.com/flexplorer/)
- [http://flexboxgrid.com/](http://flexboxgrid.com/)



## GRID

- [http://css-tricks.com/snippets/css/complete-guide-grid/](http://css-tricks.com/snippets/css/complete-guide-grid/)


## UI FRAMEWORKS
- [http://topcoat.io/](http://topcoat.io/)
- [http://getclank.com/](http://getclank.com/)


## MOBILE UI FRAMEWORKS

- [http://onsenui.io/](http://onsenui.io/) > sieht sehr fein aus - angular + topcoat (leider kein SASS)
- [http://goratchet.com](http://goratchet.com)
- [http://ionicframework.com/](http://ionicframework.com/)
- [http://code.kik.com/app/2/index.html](http://code.kik.com/app/2/index.html)


## GUIDELINES

- [http://codeguide.co/](http://codeguide.co/)
- [http://cssguidelin.es/](http://cssguidelin.es/)
- [https://gist.github.com/bobbygrace/9e961e8982f42eb91b80](https://gist.github.com/bobbygrace/9e961e8982f42eb91b80) - trello css guide
- [http://origami.ft.com/](http://origami.ft.com/)
- [http://sass-guidelin.es/](http://sass-guidelin.es/)
- [http://isobar-idev.github.io/code-standards/](http://isobar-idev.github.io/code-standards/)
- [https://github.com/necolas/idiomatic-css](https://github.com/necolas/idiomatic-css)
- [http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml](http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml)
- [https://github.com/styleguide/css](https://github.com/styleguide/css)
- [http://css-tricks.com/strategies-keeping-css-specificity-low/](http://css-tricks.com/strategies-keeping-css-specificity-low/)



## CSS

- [http://adamschwartz.co/magic-of-css/](http://adamschwartz.co/magic-of-css/)
- [http://codyhouse.co/library/](http://codyhouse.co/library/)

## MOBILE FIXED ELEMENT PROBLEM

- [http://caniuse.com/css-fixed](http://caniuse.com/css-fixed)
- [http://bradfrostweb.com/blog/mobile/fixed-position/](http://bradfrostweb.com/blog/mobile/fixed-position/)
- [http://code.tutsplus.com/tutorials/ios-5-fixed-positioning-and-content-scrolling--mobile-8332](http://code.tutsplus.com/tutorials/ios-5-fixed-positioning-and-content-scrolling--mobile-8332)

Um das Chat Input Feld am Seitenende zu halten brauchen wir wohl ein Element mit Position > Fixed und müssen dann inline scrollen?
Dafür gibt es verschiedene JS Lösungen.

- [https://github.com/ftlabs/ftscroller](https://github.com/ftlabs/ftscroller)
- [http://zynga.github.io/scroller/](http://zynga.github.io/scroller/)
- [http://iscrolljs.com/](http://iscrolljs.com/)
- [http://apdevblog.com/optimizing-webkit-overflow-scrolling/](http://apdevblog.com/optimizing-webkit-overflow-scrolling/)

 - [http://docs.telerik.com/kendo-ui/getting-started/mobile/native-scrolling](http://docs.telerik.com/kendo-ui/getting-started/mobile/native-scrolling)


## CSS LAYOUTS PRE FLEXBOX - PRE RESPONSIVE ABER IMMERNOCH NETT

- [http://matthewjamestaylor.com/blog/floating-boxes-css-layout](http://matthewjamestaylor.com/blog/floating-boxes-css-layout)
- [http://matthewjamestaylor.com/blog/keeping-footers-at-the-bottom-of-the-page](http://matthewjamestaylor.com/blog/keeping-footers-at-the-bottom-of-the-page)
- [http://matthewjamestaylor.com/blog/ultimate-multi-column-liquid-layouts-em-and-pixel-widths](http://matthewjamestaylor.com/blog/ultimate-multi-column-liquid-layouts-em-and-pixel-widths)

- [http://blog.stevensanderson.com/2011/10/05/full-height-app-layouts-a-css-trick-to-make-it-easier/](http://blog.stevensanderson.com/2011/10/05/full-height-app-layouts-a-css-trick-to-make-it-easier/)


## RESPONSIVE SLIDER - JS
- [http://bxslider.com/](http://bxslider.com/)


## JS

- Form Submit mit Enter
  - http://jsfiddle.net/McH8q/28/
  - http://jsfiddle.net/Jaganathan/6AWkH/2/
- Time Ago etc in JS
  - http://momentjs.com/


## SCROLLBAR STYLING

- [https://gist.github.com/devinrhode2/2573411]()
- [http://css-tricks.com/custom-scrollbars-in-webkit/]()


## LEARNING RESOURCES (FOR COURSE AT KHB / HFG)

- [https://designcode.io/learn](https://designcode.io/learn)
- [https://dash.generalassemb.ly](https://dash.generalassemb.ly)
- [http://teamtreehouse.com/](http://teamtreehouse.com/)
- [http://opentechschool.github.io/html-css-beginners/](http://opentechschool.github.io/html-css-beginners/)
- [http://opentechschool.github.io/js-beginners-4h-workshop-1/](http://opentechschool.github.io/js-beginners-4h-workshop-1/)
- [http://opentechschool.github.io/js-beginners-day2/](http://opentechschool.github.io/js-beginners-day2/)
- [http://www.codecademy.com/](http://www.codecademy.com/)



## STYLEGUIDES

- [http://next.fontshop.com/styleguide/globals](http://next.fontshop.com/styleguide/globals)
- [http://www.homify.de/assets/styleguide.html](http://www.homify.de/assets/styleguide.html)
- [https://github.com/styleguide](https://github.com/styleguide)

- [http://webkrauts.de/artikel/2014/living-styleguides

## STYLEGUIDE TOOLS
- [http://livingstyleguide.org/](http://livingstyleguide.org/)
- [https://github.com/hagenburger/livingstyleguide](https://github.com/hagenburger/livingstyleguide)
- [http://trulia.github.io/hologram/](http://trulia.github.io/hologram/)
- [https://github.com/kneath/kss](https://github.com/kneath/kss)
- [http://jacobrask.github.io/styledocco/](http://jacobrask.github.io/styledocco/)
- [https://github.com/pivotalexperimental/style-guide](https://github.com/pivotalexperimental/style-guide)
- [https://github.com/oreillymedia/atlas_assets](https://github.com/oreillymedia/atlas_assets)
- [https://github.com/thomasdavis/kaleistyleguide](https://github.com/thomasdavis/kaleistyleguide)

> Note to myself. Make the Styleguide based on jekyll would improve the workflow as prototyping can happen based on the same workflow.

* SASS Documentation
- [https://github.com/SassDoc/sassdoc](https://github.com/SassDoc/sassdoc)

* Reading
- [http://www.edenspiekermann.com/blog/typesetting-your-css-objects](http://www.edenspiekermann.com/blog/typesetting-your-css-objects)
- [http://www.edenspiekermann.com/blog/oocss-and-the-pagification-of-modules](http://www.edenspiekermann.com/blog/oocss-and-the-pagification-of-modules)


# ON WEB TYPOGRAPHY

## READING LIST

- [http://alistapart.com/article/more-meaningful-typography](http://alistapart.com/article/more-meaningful-typography)
- [http://hellohappy.org/beautiful-web-type/](http://hellohappy.org/beautiful-web-type/)
- [http://trentwalton.com/2013/01/07/flexible-foundations/](http://trentwalton.com/2013/01/07/flexible-foundations/)
- [http://www.abookapart.com/products/on-web-typography](http://www.abookapart.com/products/on-web-typography)
- [http://ia.net/blog/responsive-typography-the-basics/](http://ia.net/blog/responsive-typography-the-basics/)
- [http://opentypography.org/](http://opentypography.org/)
- [http://ia.net/blog/the-web-is-all-about-typography-period](http://ia.net/blog/the-web-is-all-about-typography-period)
- [http://ia.net/blog/responsive-typography/](http://ia.net/blog/responsive-typography/)
- [http://retinart.net/graphic-design/secret-law-of-page-harmony/](http://retinart.net/graphic-design/secret-law-of-page-harmony/)
- [http://read.shapeofdesignbook.com/index.html](http://read.shapeofdesignbook.com/index.html)
- [http://www.fivesimplesteps.com/products/a-practical-guide-to-designing-for-the-web](http://www.fivesimplesteps.com/products/a-practical-guide-to-designing-for-the-web)
- [http://practicaltypography.com/](http://practicaltypography.com/)
- [http://designmodo.com/web-typography/](http://designmodo.com/web-typography/)
- [http://www.elliotjaystocks.com/blog/responsive-web-typography/](http://www.elliotjaystocks.com/blog/responsive-web-typography/)


**TOOLS**
- [http://type-scale.com/](http://type-scale.com/)
- [https://typecast.com](https://typecast.com)
- [http://www.modularscale.com/](http://www.modularscale.com/)
- [http://www.gridlover.net/app/](http://www.gridlover.net/app/)
- [https://github.com/fmal/sass-baseline-rhythm](https://github.com/fmal/sass-baseline-rhythm)
- [http://typesettings.io/](http://typesettings.io/)
- [https://github.com/ianrose/typesettings](https://github.com/ianrose/typesettings)
- [https://github.com/hagenburger/livingstyleguide](https://github.com/hagenburger/livingstyleguide)

## TOOLS

- [http://www.macaw.co/](http://www.macaw.co/)
- [https://webflow.com/](https://webflow.com/)
- [http://froont.com/](http://froont.com/)
- [https://creative.adobe.com/de/products/reflow](https://creative.adobe.com/de/products/reflow)


## FRAMEWORKS

- [http://sass.fffunction.co/](http://sass.fffunction.co/)
- [http://typeplate.com/](http://typeplate.com/)



## STATIC PAGE GENERATORS
- [https://www.staticgen.com/](https://www.staticgen.com/)

## RESPONSIVE IMAGES
- [http://alistapart.com/article/responsive-images-in-practice](http://alistapart.com/article/responsive-images-in-practice)
- [https://github.com/robwierzbowski/jekyll-picture-tag](https://github.com/robwierzbowski/jekyll-picture-tag) nice - wird aber nicht mehr weiter gepflegt



## JEKYLL

- [https://github.com/ixti/jekyll-assets](https://github.com/ixti/jekyll-assets) - 
- [https://github.com/zachalbert/zachalbert.com](https://github.com/zachalbert/zachalbert.com) - fein, nicht barebones - gulp, bower
- [https://github.com/penibelst/jekyll-compress-html](https://github.com/penibelst/jekyll-compress-html) - html compress für jekyll
- [https://medium.com/design-open/becoming-a-jekyll-god-ef722e93f771](https://medium.com/design-open/becoming-a-jekyll-god-ef722e93f771) - seiten mit jekyll mit pagespeed 96 von 100 punkten
- [http://www.jekyllnow.com/](http://www.jekyllnow.com/)
- [http://www.smashingmagazine.com/2014/08/01/build-blog-jekyll-github-pages/](http://www.smashingmagazine.com/2014/08/01/build-blog-jekyll-github-pages/)
- [http://paulstamatiou.com/responsive-retina-blog-development-part-1/](http://paulstamatiou.com/responsive-retina-blog-development-part-1/)
- [http://paulstamatiou.com/responsive-retina-blog-development-part-2/](http://paulstamatiou.com/responsive-retina-blog-development-part-2/)



- [https://github.com/jensgro/Frontenddevelopment-Resources](https://github.com/jensgro/Frontenddevelopment-Resources)

- [https://github.com/dypsilon/frontend-dev-bookmarks](https://github.com/dypsilon/frontend-dev-bookmarks)




## FONTS I LIKE
- [http://www.google.com/fonts/specimen/Karla](http://www.google.com/fonts/specimen/Karla)
- [http://www.google.com/fonts/specimen/Karla](http://www.google.com/fonts/specimen/Karla)
- [http://www.google.com/fonts/specimen/Karla](http://www.google.com/fonts/specimen/Karla)




