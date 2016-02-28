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
* [snipcart](https://snipcart.com/) &ndash; online store
* [stripe](https://stripe.com)

### others
* [postmark](https://postmarkapp.com/) &ndash; email
* [apiary](https://apiary.io/) &ndash; Rapid prototype and documentation generator for APIs. 
* [roots](http://roots.cx/) &ndash; static site generator (build tool)
* [userapp](https://www.userapp.io/) &ndash; user management
* [swiftype](https://swiftype.com/) &ndash; search
* [cloudup](https://cloudup.com/) &ndash; content sharing
* [zapier](https://zapier.com/) &ndash; connect different web services
* [moltin](https://moltin.com/) &ndash; ecommmerce. Inventory management, admin UI. Have to use their cart and stuff. 

### amazon
* S3 &ndash; Simple storage service. Object storage with a web UI. Pay as you go, no minimum.
* cloudfront &ndash; CDN. Charged per gigabyte transfered.

**static hosting**  
Deploy to S3, use the amazon website to configure cloudfront.


## design

### type
* Playfair display &ndash; google font, high contrast serif
* Oswald &ndash; google font, sans-serif, news gothic like, see [http://davidtheclark.com/](http://davidtheclark.com/)

### css
* [skeleton](http://getskeleton.com/) &ndash; vanilla css boilerplate


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
