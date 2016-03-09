# notes

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [services](#services)
- [design](#design)
- [articles](#articles)
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
* [netlify](https://www.netlify.com/) &ndash; supports webhooks
* [maxCDN](https://www.maxcdn.com/)

### payments
* [stripe](https://stripe.com)

### buy things
* [snipcart](https://snipcart.com/) &ndash; online store
* [styla](http://www.styla.com/) &ndash; some kind of store thing
* [moltin](https://moltin.com/) &ndash; ecommmerce. Inventory management, admin UI. Have to use their cart and stuff. 
* [tictail](https://tictail.com/) &ndash; really good & easy, no code required, free except for payment processing

### others
* [postmark](https://postmarkapp.com/) &ndash; email
* [apiary](https://apiary.io/) &ndash; Rapid prototype and documentation generator for APIs. 
* [roots](http://roots.cx/) &ndash; static site generator (build tool)
* [userapp](https://www.userapp.io/) &ndash; user management
* [swiftype](https://swiftype.com/) &ndash; search
* [cloudup](https://cloudup.com/) &ndash; content sharing
* [zapier](https://zapier.com/) &ndash; connect different web services
* [known](https://withknown.com/) &ndash; publish to a bunch of different social sites without duplicating content

### amazon
* S3 &ndash; Simple storage service. Object storage with a web UI. Pay as you go, no minimum.
* cloudfront &ndash; CDN. Charged per gigabyte transfered.

**static hosting**  
Deploy to S3, use the amazon website to configure cloudfront.


## design

### type
* Playfair display &ndash; google font, high contrast serif
* Oswald &ndash; google font, sans-serif, news gothic like, see [http://davidtheclark.com/](http://davidtheclark.com/)
* [Italiana](https://www.google.com/fonts/specimen/Italiana) &ndash; google font. High contrast, display, deco like, only 1 weight.
* [Josephine Slab](https://www.google.com/fonts/specimen/Josefin+Slab) &ndash; Google font, slab serif, 10 styles

* [A Curated Collection of the 30 Best Google Fonts](https://www.typewolf.com/open-source-web-fonts)

### css
* [skeleton](http://getskeleton.com/) &ndash; vanilla css boilerplate
* [PostCSS the Future after Sass and Less](https://www.youtube.com/watch?v=73dl5dk9z4Q) &ndash; video, css preprocessor history, postcss design

## articles

* [Building a static CMS](http://carrot.is/coding/static_cms)
* [Static, a Revival](http://carrot.is/coding/static)
* [Why Static Website Generators Are The Next Big Thing](https://www.smashingmagazine.com/2015/11/modern-static-website-generators-next-big-thing/)
* [Obama campaign's fundraising site](http://kylerush.net/blog/meet-the-obama-campaigns-250-million-fundraising-platform/)
* [An Introduction to Static Site Generators](An Introduction to Static Site Generators)
* [New Healthcare.gov is Open, CMS-Free](https://developmentseed.org/blog/new-healthcare-gov-is-open-and-cms-free/)


## hard problems

* cache invalidation
* naming things
* css vertical centering
