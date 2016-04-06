# notes

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [services](#services)
  - [CMS](#cms)
  - [CDN](#cdn)
  - [payments](#payments)
  - [buy things](#buy-things)
  - [storage / data](#storage--data)
  - [others](#others)
  - [hosts](#hosts)
  - [amazon](#amazon)
- [design](#design)
  - [type](#type)
  - [css](#css)
- [articles](#articles)
- [javascript](#javascript)
  - [build tools](#build-tools)
  - [little modules like in lodash](#little-modules-like-in-lodash)
  - [little node tools](#little-node-tools)
  - [logging](#logging)
  - [cli](#cli)
  - [pretty cli](#pretty-cli)
  - [auth](#auth)
  - [service worker](#service-worker)
  - [DOM diffing](#dom-diffing)
- [misc](#misc)
  - [append only](#append-only)
- [hard problems](#hard-problems)

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


### others
* [postmark](https://postmarkapp.com/) &ndash; email
* [apiary](https://apiary.io/) &ndash; Rapid prototype and documentation generator for APIs. 
* [roots](http://roots.cx/) &ndash; static site generator (build tool)
* [userapp](https://www.userapp.io/) &ndash; user management
* [swiftype](https://swiftype.com/) &ndash; search
* [cloudup](https://cloudup.com/) &ndash; content sharing
* [zapier](https://zapier.com/) &ndash; connect different web services
* [known](https://withknown.com/) &ndash; publish to a bunch of different social sites
* [formkeep](https://formkeep.com) &ndash; forms
* [apigee](http://apigee.com/) &ndash; API

### hosts
[digital ocean](https://www.digitalocean.com)


### amazon
* S3 &ndash; "simple storage service". Object storage with a web UI. Pay as you go, no minimum.
* cloudfront &ndash; CDN. Charged per gigabyte transfered.
* [sns](https://aws.amazon.com/sns/) &ndash; simple notification service
* [lambda](https://aws.amazon.com/lambda/) &ndash; listen to events from other amazon services and run a function

**static hosting**  
Deploy to S3, use the amazon website to configure cloudfront.


---------------------------------------


## design

### type
* [Playfair display](https://www.google.com/fonts/specimen/Playfair+Display) &ndash; high contrast serif, 6 styles
* [Oswald](https://www.google.com/fonts/specimen/Oswald) &ndash; google font, sans-serif, news gothic like, 3 weights. see [http://davidtheclark.com/](http://davidtheclark.com/)
* [Italiana](https://www.google.com/fonts/specimen/Italiana) &ndash; google font. High contrast, display, deco like, only 1 weight.
* [Josephine Slab](https://www.google.com/fonts/specimen/Josefin+Slab) &ndash; Google font, slab serif, 10 styles
* [Merriweather](https://www.google.com/fonts/specimen/Merriweather) &ndash; serif, 8 styles
* [Lato](https://www.google.com/fonts/specimen/Lato) &ndash; sans-serif, 10 styles
* [Muli](https://www.google.com/fonts/specimen/Muli) &ndash; geometric sans-serif with single story 'a' like futura
* [Museo Sans Condensed](https://typekit.com/fonts/museo-sans-condensed) &ndash; 10 styles
* [Fira Sans 2](https://typekit.com/fonts/fira-sans-2) &ndash; really really thin sans serif

* [A Curated Collection of the 30 Best Google Fonts](https://www.typewolf.com/open-source-web-fonts)

### css
* [skeleton](http://getskeleton.com/) &ndash; vanilla css boilerplate
* [PostCSS the Future after Sass and Less](https://www.youtube.com/watch?v=73dl5dk9z4Q) &ndash; video, css preprocessor history, postcss design
* [An Introduction To PostCSS](https://www.smashingmagazine.com/2015/12/introduction-to-postcss/)
* [Grids with flexbox](https://philipwalton.github.io/solved-by-flexbox/demos/grids/)
* [flexbox froggy](http://flexboxfroggy.com/)

--------------------------------------

## articles

* [Building a static CMS](http://carrot.is/coding/static_cms)
* [Static, a Revival](http://carrot.is/coding/static)
* [Why Static Website Generators Are The Next Big Thing](https://www.smashingmagazine.com/2015/11/modern-static-website-generators-next-big-thing/)
* [Obama campaign's fundraising site](http://kylerush.net/blog/meet-the-obama-campaigns-250-million-fundraising-platform/)
* [An Introduction to Static Site Generators](An Introduction to Static Site Generators)
* [New Healthcare.gov is Open, CMS-Free](https://developmentseed.org/blog/new-healthcare-gov-is-open-and-cms-free/)
* [webapps of the future](https://github.com/substack/webapps-of-the-future) &ndash; "The door refused to open. It said, 'Five cents, please.'"


------------------------------------


## javascript

### browser
* [jump](https://github.com/callmecavs/jump.js) &ndash; scroll to places
* [tweezer](https://github.com/jaxgeller/tweezer.js) &ndash; animation thing

### build tools
* npm-run-all

### little modules like in lodash
* after
* reduce
* deep-extend

### little node tools
* brake -- throttle a stream with backpressure
* cookie-cutter -- get and set cookies client side
* monotonic-timestamp
* async-waterfall
* curry
* dom-css
* testron -- CI for browser stuff
* csjs & csjs-injectify
* nets -- http requests

### logging
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

### auth
* sodium
* passport


### service worker
* [Instant Loading Web Apps With An Application Shell Architecture](https://medium.com/google-developers/instant-loading-web-apps-with-an-application-shell-architecture-7c0c2f10c73#.51gp3l2z0) -- by Addy Osmani & Matt Gaunt
* [offline wikipedia demo](https://wiki-offline.jakearchibald.com/)


### DOM diffing

[morphdom](https://github.com/patrick-steele-idem/morphdom)

Diff the DOM vs another DOM (no virtual DOM involved).

Easier b/c *forms*. If the state in the DOM changes b/c it is mutated directly, that's fine. We don't need to preserve form state in the vdom.

No effective perfomance loss vs vdom.


------------------------


## misc

### append only

Implementations of append only logs

* [secure scuttlebutt](https://github.com/ssbc/docs)
* [forkdb](https://github.com/substack/forkdb)
* [hyperlog](https://github.com/mafintosh/hyperlog)
* [append-only-torrent](https://github.com/substack/append-only-torrent)


-------------------------


## hard problems

* cache invalidation
* naming things
* css vertical centering
