# notes

__Plus__

[See discussions](https://github.com/nichoth/notes/discussions)

--------------------------------------------------------------------------

## vscode

* `F7` / `Shift + F7` -- go to next matching Symbol
* `F8` -- go to next error / merge conflict

-------------------------------------------------------------------------

## WIP

### 2024-12-22

* [Web Authentication extensions](https://developer.mozilla.org/en-US/docs/Web/API/Web_Authentication_API/WebAuthn_extensions)

> it lets a passkey be used not just for authentication but also for deriving
> encryption keys for sensitive data on a site

--------------------------------------------------------------------------

## local first

* [The offline cookbook](https://jakearchibald.com/2014/offline-cookbook/)
* [Local First Academy](https://localfirstacademy.com/)
* [localfirst.fm](https://www.localfirst.fm/) -- A podcast about local-first software development
* [Johannes Schickling: Why Local-First? (Local-First Meetup Berlin #1)](https://youtu.be/jxuXGeMJsBU)
* [Local-first news](https://www.localfirstnews.com/)


## See also

* [the list on my website](https://nichoth.com/list/)
* [Every badge you might need](https://gist.github.com/nichoth/1fb086c5bee5cd189d66e0f87d1a4825)
* [common tasks in node JS](https://gist.github.com/nichoth/35def0bf3e37fe0dd090f40bb3e43d9b)
* [common tasks with `npm`](https://gist.github.com/nichoth/1f054534a8749cefe2034a199b588948)

## Some documents

- [iroh](./IROH.md)
- [e2ee](./End-to-End-Encryption-in-the-Browser.mht)
  + plus, [see this on the internet](https://blog.excalidraw.com/end-to-end-encryption/)
- [End-to-End Encryption in Web Apps](https://cronokirby.com/posts/2021/06/e2e_in_the_browser/)
- [some `vim` notes](./vim.md)
- [loca-first notes from discord](./LOCAL_FIRST.md)

<details><summary><h2>Contents</h2></summary>

<!-- toc -->

- [patterns](#patterns)
  * [The Baked Data architectural pattern](#the-baked-data-architectural-pattern)
- [WIP](#wip)
  * [Tues, 2024-10-29](#tues-2024-10-29)
  * [Wed, Oct 16, 2024](#wed-oct-16-2024)
  * [Mon, Oct 7, 2024](#mon-oct-7-2024)
  * [Sun, Oct 6, 2024](#sun-oct-6-2024)
  * [Sat, Oct 5, 2024](#sat-oct-5-2024)
  * [Fri, Oct 4, 2024](#fri-oct-4-2024)
  * [Thurs, Oct 3, 2024](#thurs-oct-3-2024)
  * [Web, Oct 2, 2024](#web-oct-2-2024)
  * [Tues, Oct 1, 2024](#tues-oct-1-2024)
  * [Mon, Sept 30, 2024](#mon-sept-30-2024)
  * [Web, Sept 18, 2024](#web-sept-18-2024)
  * [Mon, Sept 16, 2024](#mon-sept-16-2024)
- [changelog](#changelog)
- [license](#license)
- [June 9, 2024](#june-9-2024)

<!-- tocstop -->

</details>

## Mon, Dec 2, 2024

#CSS

* [CSS frosted glass](https://www.joshwcomeau.com/css/backdrop-filter/)

## patterns

### [The Baked Data architectural pattern](https://simonwillison.net/2021/Jul/28/baked-data/)

> provides many of the advantages of static site generators while avoiding most of their limitations

> Baked Data: bundling a read-only copy of your data alongside the code for your application, as part of the same deployment


## WIP

### Tues, 2024-10-29

### Wed, Oct 16, 2024

#music

* [Canbombe Cambá - Yamandu Costa e Martín Sued & Orquestra Assintomática](https://www.youtube.com/watch?v=6spG6w1Tfn8&ab_channel=YamanduCosta)

### Mon, Oct 7, 2024

#crypto

* [Ed25519 to Curve25519](https://libsodium.gitbook.io/doc/advanced/ed25519-curve25519) -- that link from @getify.
   - [An example in use](https://github.com/mylofi/local-data-lock/blob/ac2a28e64b6666d4bd6a142e97a71ad2745fe18a/src/ldl.js#L538)

### Sun, Oct 6, 2024

#local-first
#crypto

* add [local-first notes](./LOCAL_FIRST.md) from discord
* [rfc9420](https://github.com/mlswg/mls-protocol/blob/1a441b8af19f2dd6dc0b7301a9c788bb8985090f/rfc9420.md)

### Sat, Oct 5, 2024

#CSS #web

* [CSS and Network Performance](https://csswizardry.com/2018/11/css-and-network-performance/)
* [Conditionally loading resources with media queries](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link#conditionally_loading_resources_with_media_queries)

Use a media query in the `link` tag, and separate the CSS by media query, so
you only need to download the relevant CSS.

### Fri, Oct 4, 2024

#JS
#web
#design

* [Leader election in browser tabs, the easy way](https://greenvitriol.com/posts/browser-leader)
* [component.gallery](https://component.gallery/)

>
> Designed to be a reference for anyone building component-based user
> interfaces, The Component Gallery is an up-to-date repository of interface
> components based on examples from the world of design systems.
>

### Thurs, Oct 3, 2024

#web

* [What is atproto.com good for?](https://bnewbold.net/2022/atproto_thoughts/)


#music

* Alabaster DePlume

#JS #server

* [Hono Web application framework](https://hono.dev/)
  + [github](https://github.com/honojs/hono)
* [Nitro -- Next Generation Server Toolkit](https://nitro.unjs.io/)
  + [github](https://github.com/unjs/nitro)
* [h3 -- The Web Framework for Modern JavaScript Era](https://h3.unjs.io/)
  + [github](https://github.com/unjs/h3)
* [unjs](https://unjs.io/)

### Web, Oct 2, 2024

#webcomponent

* [The different ways to instantiate a Web Component](https://gomakethings.com/the-different-ways-to-instantiate-a-web-component/#inside-the-constructor)

### Tues, Oct 1, 2024

#css
#webcomponent #web-component

* [CSS Masonry & CSS Grid](https://css-tricks.com/css-masonry-css-grid/)
* [CSS ::part selector](https://developer.mozilla.org/en-US/docs/Web/CSS/::part)

### Mon, Sept 30, 2024

* [Git from the inside out](https://maryrosecook.com/blog/post/git-from-the-inside-out)
* [The Cloud Is a Prison. Can the Local-First Software Movement Set Us Free?](https://www.wired.com/story/the-cloud-is-a-prison-can-the-local-first-software-movement-set-us-free/) (local-first in Wired magazine)
* [CRDTs Turned Inside Out](https://interjectedfuture.com/crdts-turned-inside-out/)

#web-components #JS

* [Requirements for custom element constructors and reactions](https://html.spec.whatwg.org/multipage/custom-elements.html#custom-element-conformance)
* [Using custom elements](https://developer.mozilla.org/en-US/docs/Web/API/Web_components/Using_custom_elements#types_of_custom_element)
* [The Great Divide](https://css-tricks.com/the-great-divide/)

--------------

* [Web components are okay](https://nolanlawson.com/2024/09/28/web-components-are-okay/)

#JS

#### create an array of length

```js
Array.from({ length: 5 }, (v, i) => i)
// => [0, 1, 2, 3, 4]
```

#### get an array of the alphabet

```js
Array.from({ length: 26 }).map((_, i) => String.fromCharCode(i + 1 + 64))
```

### Web, Sept 18, 2024

* [Iroh — IPFS reimagined](https://youtu.be/9jR9EWZ2bO8)

  > Content discovery is the hard part.

  > You want a global view into the world -- who has the answer to this query?

  > something older than 24 hours on the IPFS network, that's not on the gateway, that's hard to get

  > high latency

  > too many layers

The hidden killer of many projects -- too many layers.


* [see this note via iroh discord](./IROH.md)


### Mon, Sept 16, 2024

* [HTML5 with storing files in IndexedDB](https://robnyman.github.io/html5demos/indexeddb/)
  - [html5demos/indexeddb/js/base.js](https://github.com/robnyman/robnyman.github.com/blob/master/html5demos/indexeddb/js/base.js)
* [robnyman.github.io/camera-api](https://robnyman.github.io/camera-api/)
* [Blobs and More: Storing Images and Files in IndexedDB](https://dzone.com/articles/blobs-and-more-storing-images)
* [Aljoscha Meyer & Sam Gwilym - Earthstar + Willow](https://nlnet.nl/project/Earthstar/interview.html) — an interview by nlnet
* [signal protocol — Diffie-Hellman ratchet](https://signal.org/docs/specifications/doubleratchet/#kdf-chains)
* [The Garden and the Stream: A Technopastoral](https://hapgood.us/2015/10/17/the-garden-and-the-stream-a-technopastoral/)
* [Of Digital Streams, Campfires and Gardens](https://tomcritchlow.com/2018/10/10/of-gardens-and-wikis/)

-----------------------------

* [Hyper Hyper Space: Conclusions and ideas for building p2p secure data sync](https://www.hyperhyperspace.org/report.html)
* [messwithdns.net](https://messwithdns.net/)
* [maxnowack/signaldb](https://github.com/maxnowack/signaldb)
* [Rebuilding the Web We Lost](https://www.anildash.com//2012/12/18/rebuilding_the_web_we_lost/)
* [More on Streams vs. Pages](https://www.anildash.com//2012/08/15/more_on_streams_vs_pages/)
* [Stop Publishing Web Pages](https://www.anildash.com//2012/08/14/stop_publishing_web_pages/)
* [Don’t Be Evil: Fred Turner on Utopias, Frontiers, and Brogrammers](https://logicmag.io/justice/fred-turner-dont-be-evil/)
* [MOTIVATED: Playing with MP4 Metadata](https://whtwnd.com/msh.bsky.social/3l42sodfdzh22)
* [signal — kdf chains](https://signal.org/docs/specifications/doubleratchet/#kdf-chains)
* [Understanding HKDF](https://soatok.blog/2021/11/17/understanding-hkdf/) — a dhole moment
* [dajiaji/hpke-js](https://github.com/dajiaji/hpke-js/tree/main)
* [Everything you wanted to know about Elliptic Curve Cryptography](https://fission.codes/blog/everything-you-wanted-to-know-about-elliptic-curve-cryptography/)

-------------

* [esbuild bundle analyzer](https://esbuild.github.io/analyze/)
* [electric-sql/pglite](https://github.com/electric-sql/pglite)
* [pglite.dev](https://pglite.dev/)

## changelog

* [common changelog](https://common-changelog.org/)
* [keep a changelog](https://keepachangelog.com/en/1.0.0/)

## license

* A badge for [the Polyform Shield license](https://polyformproject.org/licenses/shield/1.0.0/)

A link to the badge: [badge](https://github.com/nichoth/badge?tab=readme-ov-file#polyform-shield-license)

Looks like this: ![Polyform shield badge](https://nichoth.github.io/badge/polyform-shield.svg)

---------------------------

## June 9, 2024

* [vella.ai](https://vella.ai/auth/) -- Local-First Auth

----------

* [Elasticlunr.js](http://elasticlunr.com/) -- Lightweight full-text search engine in Javascript for browser search and offline search
