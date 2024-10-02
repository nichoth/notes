# notes

[See discussions](https://github.com/nichoth/notes/discussions)

See also, [the list on my website](https://nichoth.com/list/)

## contents

- [iroh](./IROH.md)
- [e2ee](./End-to-End-Encryption-in-the-Browser.mht)
  + [see this on the internet](https://blog.excalidraw.com/end-to-end-encryption/)
- [End-to-End Encryption in Web Apps](https://cronokirby.com/posts/2021/06/e2e_in_the_browser/)

-----------------------------

<!-- toc -->

- [WIP](#wip)
  * [Web, Oct 2](#web-oct-2)
  * [Tues, Oct 1](#tues-oct-1)
  * [Mon, Sept 30, 2024](#mon-sept-30-2024)
  * [Web, Sept 18, 2024](#web-sept-18-2024)
  * [Mon, Sept 16, 2024](#mon-sept-16-2024)
- [changelog](#changelog)
- [June 9, 2024](#june-9-2024)

<!-- tocstop -->

## WIP

### Web, Oct 2

#webcomponent

* [The different ways to instantiate a Web Component](https://gomakethings.com/the-different-ways-to-instantiate-a-web-component/#inside-the-constructor)

### Tues, Oct 1

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

Plus, a badge, for [Polyform Shield license](https://polyformproject.org/licenses/shield/1.0.0/).

[badge](https://github.com/nichoth/badge?tab=readme-ov-file#polyform-shield-license)

---------------------------

## June 9, 2024

* [vella.ai](https://vella.ai/auth/) -- Local-First Auth

----------

* [Elasticlunr.js](http://elasticlunr.com/) -- Lightweight full-text search engine in Javascript for browser search and offline search
