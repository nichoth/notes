# notes

[See discussions](https://github.com/nichoth/notes/discussions)

## the web

* [Syndicating Content to Twitter](https://mxb.dev/blog/syndicating-content-to-twitter-with-netlify-functions/) via netlify functions
* [The IndieWeb for Everyone](https://mxb.dev/blog/the-indieweb-for-everyone/)
* [Webmention](https://indieweb.org/Webmention)
* [backfeed](https://indieweb.org/backfeed)
* [webmention.io](https://webmention.io/) -- a hosted service created to easily receive webmentions on any web page
* [indieAuth.com](https://indieauth.com/)
* [POSSE](https://indieweb.org/POSSE) -- Publish (on your) Own Site, Syndicate Elsewhere
* [note](https://indieweb.org/note)

* [Signaling as a Service](https://julian.digital/2020/03/28/signaling-as-a-service/)

> A social network like Path attempted to limit your social graph size to the Dunbar number, capping your social capital accumulation potential and capping the distribution of your posts. The exchange, they hoped, was some greater transparency, more genuine self-expression. The anti-Facebook. Unfortunately, as social capital theory might predict, Path did indeed succeed in becoming the anti-Facebook: a network without enough users. Some businesses work best at scale, and if you believe that people want to accumulate social capital as efficiently as possible, putting a bound on how much they can earn is a challenging business model, as dark as that may be.

> Deliberately limiting the number of people who can join a network (e.g. by charging a membership fee) creates scarcity which in turns makes the network more interesting. Network membership becomes the signal message.

* [gist of deploy succeeded function](https://gist.github.com/maxboeck/77c3c8e244f190147cca2f7383d5f183) — for some sort of notes feed
* [brid.gy](https://brid.gy/) — connects your web site to social media.

-------

* [Better Living Through Caching](https://www.netlify.com/blog/2017/02/23/better-living-through-caching/)

-------

## PWA
* [Add to home screen]()https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Add_to_home_screen
* [Make them installable](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Installable_PWAs)

### See also
* [web manifest](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Add_to_home_screen#manifest)
* [service worker](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API)
* [A link in HTML](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Add_to_home_screen#link_the_html_to_the_manifest)

### Cloudinary + PWA
* https://cloudinary.com/labs/cloudinary-serviceworker
* https://gist.github.com/ukmadlz/5d55ca5f6c0d4233e193caad47403fe4

### Lazy loading images
* [MDN – Lazy Loading](https://developer.mozilla.org/en-US/docs/Web/Performance/Lazy_loading#loading_attribute)

> The [loading](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img#loading) attribute on an [<img>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img) element (or the [loading](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe#loading) attribute on an [<iframe>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe)) can be used to instruct the browser to defer loading of images/iframes that are off-screen until the user scrolls near them.

```html
<img src="image.jpg" alt="..." loading="lazy" />
```

* [web.dev](https://web.dev/browser-level-image-lazy-loading/)

> If you want to increase the fetch priority of an important image (for example the LCP image), then [Fetch Priority](https://web.dev/fetch-priority/) should be used with fetchpriority="high".

> Note that an image with loading="lazy" and fetchpriority="high" will still be delayed while it is off-screen, and then fetched with a high priority when it is nearly within the viewport. It would likely be fetched with a high priority in this case anyway, so this combination should not really be needed nor used.

-------

## frontend
* [pwa article](https://medium.com/google-developers/instant-loading-web-apps-with-an-application-shell-architecture-7c0c2f10c73#.51gp3l2z0)
* [islands architecture](https://jasonformat.com/islands-architecture/)
* [fresh](https://fresh.deno.dev/) — the framework for deno
* [Things you forgot (or never knew) because of React](https://joshcollinsworth.com/blog/antiquated-react)

### signals
* [mastodon.social/@developit — Persisted Signals](https://mastodon.social/@developit/110911126736335349)
  - [persisted signal gist](https://gist.github.com/developit/baa45015a607877a9a9e2697fb32ab8b)

* [signal-utils gist](https://gist.github.com/developit/a72311c247756f24da5b22d19c9dad48)

### dialog element
* [Dialog :: Stuff browsers give for free](https://www.youtube.com/watch?v=y8HjQETqrOM&ab_channel=DaveCross)
A nice video explanation of `dialog` element.

* Hidde's Blog — [Dialogs and popovers seem similar. How are they different?](https://hidde.blog/dialog-modal-popover-differences/)
> In addition to the [<dialog> element](https://html.spec.whatwg.org/dev/interactive-elements.html#the-dialog-element), HTML now has a [popover attribute](https://html.spec.whatwg.org/dev/popover.html#the-popover-attribute). This post goes into the differences between dialogs, popovers, overlays and disclosure widgets. We'll also look at what it means when an element is modal. All somewhat related concepts

-------

## p2p

* [Holepunching finally explained](https://youtu.be/nuK_PqvTQxo?t=2010)
* [LoFi discord -- talk about p2p](https://discord.com/channels/929781625473073245/1087795275365625917/1123653729867006134)
* [the pushpin paper](https://www.inkandswitch.com/pushpin/#nat-traversal) -- NAT traversal
* [Mathias Buus / Hypercore protocol & Holepunch](https://www.youtube.com/watch?v=nuK_PqvTQxo&t=2010s&ab_channel=WizardAmigos)
* [discord discussion of](https://discord.com/channels/776925030549291059/795521196677922876/1123661229894946816) a video — [Mathias Buus / Hypercore protocol & Holepunch](https://youtu.be/nuK_PqvTQxo?t=2260)
* [p2panda](https://p2panda.org/)

-------

## offline

* [Local-first software -- Peter Van Hardenberg](https://www.youtube.com/watch?v=KrPsyr8Ig6M)
* [The offline cookbook](https://jakearchibald.com/2014/offline-cookbook/)
* [The disintermediated web - Substack](https://www.youtube.com/watch?v=6jcQoSraHcw&list=PL0CdgOSSGlBYnHAl_DZoy9BWvdVQjNKE2&index=4&ab_channel=NearForm)

### tools
* [Electric SQL](https://electric-sql.com/) — Build reactive, realtime, local-first apps directly on Postgres.
* [PartyKit, meet TinyBase](https://blog.partykit.io/posts/partykit-meet-tinybase)

> [TinyBase](https://tinybase.org/), a reactive data store for local-first apps. It lets you store structured data and application state in memory, and provides a reactive UI so that you can build fast web experiences that work both online and offline.

> This integration allows you to enjoy the benefits of both a “local-first” architecture and a “sharing-first” platform. 

[see demo](https://beta.tinybase.org/demos/todo-app/todo-app-v6-collaboration/)

* [starter repo](https://github.com/tinyplex/tinybase-ts-react-partykit)
* [partykit](https://www.partykit.io/)

> PartyKit simplifies developing multiplayer applications. 

> PartyKit will handle operational complexity and real-time infrastructure scaling.

> Each PartyKit server (also known as a Party), is backed by a Cloudflare [Durable Object](https://docs.partykit.io/glossary/#durable-object).

> you can also connect to a Party using standard WebSockets, enabling real-time push between client and the party instance (also known as “room”)

> Parties are so lightweight that we can spin them up with practically zero start-up time. In this regard, they are similar to a serverless function.

[partykit — Persisting state into storage](https://docs.partykit.io/guides/persisting-state-into-storage#keeping-data-between-server-restarts)

> Persisting data to disk is optional as PartyKit servers also allow you to keep in-memory state. It is, however, necessary, when you want the stored data to persist between server restarts.

> Server restarts happen when:

> * You re-deploy the party using partykit deploy.
> * Having opted into [Hibernation](https://docs.partykit.io/guides/scaling-partykit-servers-with-hibernation/), the server is currently not processing messages.
> * There’s an unexpected error in the PartyKit runtime (for example, a hardware fault).
> * The server reaches its maximum lifetime.

-------

## analytics
* [plausible](https://plausible.io/) -- Easy to use and privacy-friendly Google Analytics alternative

