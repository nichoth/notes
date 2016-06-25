# notes

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [services](#services)
  - [CMS](#cms)
  - [CDN](#cdn)
  - [payments](#payments)
  - [buy things](#buy-things)
  - [storage / data](#storage--data)
  - [search](#search)
  - [others](#others)
  - [hosts](#hosts)
  - [amazon](#amazon)
  - [static sites](#static-sites)
- [design](#design)
  - [type](#type)
  - [css](#css)
- [articles](#articles)
- [javascript](#javascript)
  - [browser](#browser)
  - [build & dev tools](#build-&-dev-tools)
  - [little modules like in lodash](#little-modules-like-in-lodash)
  - [node tools](#node-tools)
  - [logging](#logging)
  - [cli](#cli)
  - [pretty cli](#pretty-cli)
  - [auth](#auth)
  - [service worker](#service-worker)
  - [View layer](#view-layer)
- [git](#git)
- [misc](#misc)
  - [append only logs](#append-only-logs)
- [hard problems](#hard-problems)
- [cool shit](#cool-shit)
- [to read](#to-read)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## services

### CMS
* [cloudcannon](http://cloudcannon.com/) &ndash; supports Jekyll or vanilla static
* [contentful](https://www.contentful.com/)
* [siteleaf](http://www.siteleaf.com/)
* [gathercontent](https://gathercontent.com/)
* [prismic](https://prismic.io/)

### CDN
* [netlify](https://www.netlify.com/) &ndash; easy webhooks
* [maxCDN](https://www.maxcdn.com/)

### payments
* [stripe](https://stripe.com)

### buy things
* [snipcart](https://snipcart.com/) &ndash; online store
* [styla](http://www.styla.com/) &ndash; some kind of store thing
* [moltin](https://moltin.com/) &ndash; ecommmerce. Inventory management, admin UI. Have to use their cart and stuff. 
* [tictail](https://tictail.com/) &ndash; really good & easy, no code required, free except for payment processing

### storage / data
* [remotestorage.io](https://remotestorage.io/) &ndash; sync, offline
* [kinto](http://kinto.readthedocs.org/en/latest/overview.html#why-use-kinto) &ndash; sync, offline
* [hoodie](Hoodie) &ndash; offline, sync, facade for any backend

### search
* [algolia](https://www.algolia.com/) 
* [swiftype](https://swiftype.com/) &ndash; search

### others
* [postmark](https://postmarkapp.com/) &ndash; email
* [apiary](https://apiary.io/) &ndash; Rapid prototype and documentation generator for APIs. 
* [roots](http://roots.cx/) &ndash; static site generator (build tool)
* [userapp](https://www.userapp.io/) &ndash; user management
* [cloudup](https://cloudup.com/) &ndash; content sharing
* [zapier](https://zapier.com/) &ndash; connect different web services
* [known](https://withknown.com/) &ndash; publish to a bunch of different social sites
* [formkeep](https://formkeep.com) &ndash; forms
* [apigee](http://apigee.com/) &ndash; API
* [pingdom](https://tools.pingdom.com/) &ndash; measure page load performance

### hosts
[digital ocean](https://www.digitalocean.com)

### amazon
* S3 &ndash; "simple storage service". Object storage with a web UI. Pay as you go, no minimum.
* cloudfront &ndash; CDN. Charged per gigabyte transfered.
* [sns](https://aws.amazon.com/sns/) &ndash; simple notification service
* [lambda](https://aws.amazon.com/lambda/) &ndash; listen to events from other amazon services and run a function

**static hosting**  
Deploy to S3, use the amazon website to configure cloudfront.


### static sites
* [surge](http://surge.sh)
* [staticland](https://static.land/)

---------------------------------------


## design

### type
* [Playfair display](https://www.google.com/fonts/specimen/Playfair+Display) &ndash; high contrast serif, 6 styles
* [Oswald](https://www.google.com/fonts/specimen/Oswald) &ndash; google font, sans-serif, news gothic like, 3 weights. see [http://davidtheclark.com/](http://davidtheclark.com/)
* [Josephine Slab](https://www.google.com/fonts/specimen/Josefin+Slab) &ndash; Google font, slab serif, 10 styles
* [Merriweather](https://www.google.com/fonts/specimen/Merriweather) &ndash; serif, 8 styles
* [Lato](https://www.google.com/fonts/specimen/Lato) &ndash; sans-serif, 10 styles, thin weights
* [Muli](https://www.google.com/fonts/specimen/Muli) &ndash; geometric sans-serif with single story 'a' like futura
* [Museo Sans Condensed](https://typekit.com/fonts/museo-sans-condensed) &ndash; 10 styles
* [Fira Sans 2](https://typekit.com/fonts/fira-sans-2) &ndash; really really thin sans serif
* [Martel Sans](https://www.google.com/fonts/specimen/Martel+Sans) &ndash; 7 weights, contrast, diagonal axis
* [Poppins](https://www.google.com/fonts/specimen/Poppins) &ndash; Geometric sans-serif, 5 weights, no italic

#### display
* [Italiana](https://www.google.com/fonts/specimen/Italiana) &ndash; google font. High contrast, display, deco like, only 1 weight.
* [Poiret One](https://www.google.com/fonts/specimen/Poiret+One) &ndash; thin oblique sans serif, only one weight
* [Limelight](https://www.google.com/fonts/specimen/Limelight) &ndash; art decco movie theater, 1 weight
* [Arapey](https://www.google.com/fonts/specimen/Arapey) &ndash; serif, kind of high contrast. Like Didot when it's drunk. 2 styles &ndash; normal and italic.
* [Prata](https://www.google.com/fonts/specimen/Prata) &ndash; serif high contrast, like Didot. 1 weight
* [Suranna](https://www.google.com/fonts/specimen/Suranna) &ndash; serif high contrast, like Didot. 1 weight.
* [Bentham](https://www.google.com/fonts/specimen/Bentham) &ndash; serif high contrast. 1 style.
* [Old Standard TT](https://www.google.com/fonts/specimen/Old+Standard+TT) &ndash; high contrast serif. 3 styles &ndash; normal, bold, italic
* [IM Fell English](https://www.google.com/fonts/specimen/IM+Fell+English) &ndash; Old looking serif

* [A Curated Collection of the 30 Best Google Fonts](https://www.typewolf.com/open-source-web-fonts)

### css
* [skeleton](http://getskeleton.com/) &ndash; vanilla css boilerplate
* [PostCSS the Future after Sass and Less](https://www.youtube.com/watch?v=73dl5dk9z4Q) &ndash; video, css preprocessor history, postcss design
* [An Introduction To PostCSS](https://www.smashingmagazine.com/2015/12/introduction-to-postcss/)
* [Grids with flexbox](https://philipwalton.github.io/solved-by-flexbox/demos/grids/)
* [flexbox froggy](http://flexboxfroggy.com/)
* [flexbox codepen](http://codepen.io/osublake/full/dMLQJr/)

#### shapes, clipping, svg
* [clippy](http://bennettfeely.com/clippy/) &ndash; make css clipping shapes with a gui tool
* [smashing article](https://www.smashingmagazine.com/2015/05/creating-responsive-shapes-with-clip-path/) &ndash; css and svg clipping paths
* [svg responsive, viewbox](https://docs.google.com/presentation/d/1Iuvf3saPCJepVJBDNNDSmSsA0_rwtRYehSmmSSLYFVQ/pub?start=false&loop=false&delayms=3000&slide=id.g18168351a_07) &ndash; how to use viewbox for responsive svgs
* [svg animating paths](https://docs.google.com/presentation/d/1Iuvf3saPCJepVJBDNNDSmSsA0_rwtRYehSmmSSLYFVQ/pub?start=false&loop=false&delayms=3000&slide=id.g34112647d_0121) &ndash; use snap.svg

--------------------------------------

## articles

* [Building a static CMS](http://carrot.is/coding/static_cms)
* [Static, a Revival](http://carrot.is/coding/static)
* [Why Static Website Generators Are The Next Big Thing](https://www.smashingmagazine.com/2015/11/modern-static-website-generators-next-big-thing/)
* [Obama campaign's fundraising site](http://kylerush.net/blog/meet-the-obama-campaigns-250-million-fundraising-platform/)
* [An Introduction to Static Site Generators](An Introduction to Static Site Generators)
* [New Healthcare.gov is Open, CMS-Free](https://developmentseed.org/blog/new-healthcare-gov-is-open-and-cms-free/)
* [webapps of the future](https://github.com/substack/webapps-of-the-future) &ndash; "The door refused to open. It said, 'Five cents, please.'"
* [Pokedex](http://www.pocketjavascript.com/blog/2015/11/23/introducing-pokedex-org) -- offline, web worker, service worker
* [UNIDIRECTIONAL USER INTERFACE ARCHITECTURES](http://staltz.com/unidirectional-user-interface-architectures.html)

------------------------------------


## javascript

### browser
* [jump](https://github.com/callmecavs/jump.js) &ndash; scroll to places
* [tweezer](https://github.com/jaxgeller/tweezer.js) &ndash; animation thing
* dom101 - utilities like in jQuery, but modular style
* [remy's polyfills](https://github.com/remy/polyfills)
* mousetrap -- keyboard shortcuts

### build & dev tools
* npm-run-all -- run many scripts at once
* scripty -- manage npm scripts
* bundleify -- preset transforms for browserify
* es2020 -- only use what you need in es6
* bundle-collapser -- optimize file size in browserify
* insert-css -- insert a string of css into the file
* standard -- easy code style
* csjs-extractify -- extract csjs into an external css bundle

### little modules like in lodash
* arrify
* after
* reduce
* deep-extend
* array-range
* object.pick
* object-values

### node tools
* restify -- easy server
* brake -- throttle a stream with backpressure
* cookie-cutter -- get and set cookies client side
* monotonic-timestamp
* async-waterfall
* curry
* dom-css
* testron -- CI for browser stuff
* csjs & csjs-injectify
* nets -- http requests
* xhr -- like nets
* [EventEmitter2](https://github.com/asyncly/EventEmitter2) -- deluxe events
* multipipe -- nice streams
* chloride -- cryptography
* semantic-release
* drag-and-drop-files
* nock -- http server mock
* nodemailer -- email

### logging
* pino
* bole

### cli
* configstore
* rc
* meow
* yargs
* moniker -- generate random names
* [more](https://github.com/sindresorhus/awesome-nodejs#command-line-utilities)

### pretty cli
* garnish
* chalk
* x256
* terminal-menu
* inquirer
* prompt
* bistre -- print colourful bole logs
* ora -- loading spinner
* cli-spinners
* log-update -- animations
* progress

### auth
* sodium
* passport


### service worker
* [Instant Loading Web Apps With An Application Shell Architecture](https://medium.com/google-developers/instant-loading-web-apps-with-an-application-shell-architecture-7c0c2f10c73#.51gp3l2z0) -- by Addy Osmani & Matt Gaunt
* [offline wikipedia demo](https://wiki-offline.jakearchibald.com/)


### View layer

* [morphdom](https://github.com/patrick-steele-idem/morphdom)
* [skatejs](https://github.com/skatejs/skatejs) -- component stuff
* [throw-down](https://github.com/silentcicero/throw-down) -- dom node lifecycle
* [marko](https://github.com/marko-js/marko) -- template thing

-----------------------

## git

Merge conflicts

```sh
$ git checkout --ours <file>
$ git checkout --theirs <file>
```

------------------------

## misc


### append only logs

* [secure scuttlebutt](https://github.com/ssbc/docs)
* [forkdb](https://github.com/substack/forkdb)
* [hyperlog](https://github.com/mafintosh/hyperlog)
* [append-only-torrent](https://github.com/substack/append-only-torrent)


-------------------------


## hard problems

* cache invalidation
* naming things
* css vertical centering


## cool shit

* cli-weather
* [nlp_compromise](https://github.com/nlp-compromise/nlp_compromise)
* [p2p workshop](https://p2p-workshop.mafintosh.com/)
* [how2](https://www.npmjs.com/package/how2)
* [distributed patterns workshop](http://yoshuawuyts.com/workshop-distributed-patterns/build/00.html)


## to read
[EventSource](https://developer.mozilla.org/en-US/docs/Web/API/EventSource)



