# notes

## cryptography

### double ratchet

* [Double ratchet algorithm: The ping-pong game encrypting Signal and WhatsApp](https://www.youtube.com/watch?v=7uEeE3TUqmU&ab_channel=ChalkTalk) — a nice video explanation
* [matheus23/wnfs2/src/fs/data/private/spiralratchet.ts](https://github.com/oddsdk/ts-odd/blob/matheus23/wnfs2/src/fs/data/private/spiralratchet.ts) — implementation in ts
* see [Brooklyn Zelenka Strange Loop talk about skip ratchet](https://www.youtube.com/watch?v=3UjQd-JnMrQ&t=178s&ab_channel=StrangeLoopConference)

**ratchet 1**
Create a new key per message. This creates "forward secrecy", meaning you can't get previous keys if you learn the current key.

**ratchet 2**
Each time we send a message, we create a new keypair. We embed the public side in the message, and use the private side to do a Diffie-Hellman exchange with the recipient's most recent public key, creating a new secret key for this message. Encrypt the message with this new secret key. 

This creates the opposite ratchet. Meaning you cannot read future messages if you learn the current key.

The double ratchet depends on each user having a public & private key.

see [Sending the initial message](https://www.signal.org/docs/specifications/x3dh/#sending-the-initial-message)

### MLS
[Messaging layer security: Encrypting a group chat](https://www.youtube.com/watch?v=FESp2LHd42U&ab_channel=ChalkTalk)

### [wikipedia diffie hellman](https://en.wikipedia.org/wiki/Diffie%E2%80%93Hellman_key_exchange#Triple_Diffie-Hellman_(3-DH))

> It is also possible to use Diffie–Hellman as part of a [public key infrastructure](https://en.wikipedia.org/wiki/Public_key_infrastructure), allowing Bob to encrypt a message so that only Alice will be able to decrypt it, with no prior communication between them other than Bob having trusted knowledge of Alice's public key.

### [wikipedia double ratchet](https://en.wikipedia.org/wiki/Double_Ratchet_Algorithm)

> the Double Ratchet Algorithm is a [key](https://en.wikipedia.org/wiki/Key_(cryptography)) management algorithm

> It combines a cryptographic so-called "ratchet" based on the [Diffie–Hellman key exchange](https://en.wikipedia.org/wiki/Diffie%E2%80%93Hellman_key_exchange) (DH) and a ratchet based on a [key derivation function](https://en.wikipedia.org/wiki/Key_derivation_function) (KDF), such as a [hash function](https://en.wikipedia.org/wiki/Hash_function), and is therefore called a double ratchet

-------

### [signal.org/blog/advanced-ratcheting](https://signal.org/blog/advanced-ratcheting/)

> OTR takes things a step further by continuously ratcheting the key material forward during the course of a session. 

> Alice will use the advertised and acknowledged key the next time she sends a message.

-------

### [blog.excalidraw.com/end-to-end-encryption](https://blog.excalidraw.com/end-to-end-encryption/)

the premise of https://wormhole.app/ — put a private key after the `#` in the URL 

## data structures
* [itsy-bitsy-data-structures.js](https://github.com/jamiebuilds/itsy-bitsy-data-structures/blob/master/itsy-bitsy-data-structures.js)

## pwa
* [pwa article](https://medium.com/google-developers/instant-loading-web-apps-with-an-application-shell-architecture-7c0c2f10c73#.51gp3l2z0)

## analytics
* [plausible](https://plausible.io/) -- Easy to use and privacy-friendly Google Analytics alternative

## offline
* [Local-first software -- Peter Van Hardenberg](https://www.youtube.com/watch?v=KrPsyr8Ig6M)
* [The offline cookbook](https://jakearchibald.com/2014/offline-cookbook/)
* [The disintermediated web - Substack](https://www.youtube.com/watch?v=6jcQoSraHcw&list=PL0CdgOSSGlBYnHAl_DZoy9BWvdVQjNKE2&index=4&ab_channel=NearForm)

## database
* [ImmortalDB](https://github.com/gruns/ImmortalDB) -- a resilient key-value store for the browser
* [Verdant](https://github.com/a-type/verdant) -- An IndexedDB-powered database and data sync solution for sustainable, human, local-first web apps.

## p2p
* [Holepunching finally explained](https://youtu.be/nuK_PqvTQxo?t=2010)
* [LoFi discord -- talk about p2p](https://discord.com/channels/929781625473073245/1087795275365625917/1123653729867006134)
* [the pushpin paper](https://www.inkandswitch.com/pushpin/#nat-traversal) -- NAT traversal
* [Mathias Buus / Hypercore protocol & Holepunch](https://www.youtube.com/watch?v=nuK_PqvTQxo&t=2010s&ab_channel=WizardAmigos)

## frontend
* [mastodon.social/@developit — Persisted Signals](https://mastodon.social/@developit/110911126736335349)
  - [persisted signal gist](https://gist.github.com/developit/baa45015a607877a9a9e2697fb32ab8b)

* [signal-utils gist](https://gist.github.com/developit/a72311c247756f24da5b22d19c9dad48)

### dialog element
* [Dialog :: Stuff browsers give for free](https://www.youtube.com/watch?v=y8HjQETqrOM&ab_channel=DaveCross)
A nice video explanation of `dialog` element.

* Hidde's Blog — [Dialogs and popovers seem similar. How are they different?](https://hidde.blog/dialog-modal-popover-differences/)
> In addition to the [<dialog> element](https://html.spec.whatwg.org/dev/interactive-elements.html#the-dialog-element), HTML now has a [popover attribute](https://html.spec.whatwg.org/dev/popover.html#the-popover-attribute). This post goes into the differences between dialogs, popovers, overlays and disclosure widgets. We'll also look at what it means when an element is modal. All somewhat related concepts

## streams
* [@gwil being helpful in discord](https://discord.com/channels/613255095106142219/730562221612073041/1082543804076269628) about whatwg streams

## the web
* [Syndicating Content to Twitter](https://mxb.dev/blog/syndicating-content-to-twitter-with-netlify-functions/) via netlify functions
* [The IndieWeb for Everyone](https://mxb.dev/blog/the-indieweb-for-everyone/)
* [Webmention](https://indieweb.org/Webmention)
* [backfeed](https://indieweb.org/backfeed)
* [webmention.io](https://webmention.io/) -- a hosted service created to easily receive webmentions on any web page
* [indieAuth.com](https://indieauth.com/)
* [POSSE](https://indieweb.org/POSSE) -- Publish (on your) Own Site, Syndicate Elsewhere
* [note](https://indieweb.org/note)

## misc

* [socketsupply/treehash](https://github.com/socketsupply/treehash) — Hash a large file into a tree.
This makes it possible to verify just a portion of the file, if you know the necessary tree hashes.
* [The anthesis web: Anytype raises $13.4M to restore the Internet
](https://tech.eu/2023/08/23/anytype-raises-13-4m-decentralised-web/)

* [Signaling as a Service](https://julian.digital/2020/03/28/signaling-as-a-service/)

> A social network like Path attempted to limit your social graph size to the Dunbar number, capping your social capital accumulation potential and capping the distribution of your posts. The exchange, they hoped, was some greater transparency, more genuine self-expression. The anti-Facebook. Unfortunately, as social capital theory might predict, Path did indeed succeed in becoming the anti-Facebook: a network without enough users. Some businesses work best at scale, and if you believe that people want to accumulate social capital as efficiently as possible, putting a bound on how much they can earn is a challenging business model, as dark as that may be.

> Deliberately limiting the number of people who can join a network (e.g. by charging a membership fee) creates scarcity which in turns makes the network more interesting. Network membership becomes the signal message.

-------

* [Make RPC calls over a Kademlia based DHT](https://github.com/mafintosh/dht-rpc)


## vintage video
* [npmCamp 2016 - Registry Design Patterns by CJ Silverio](https://www.youtube.com/watch?v=WucjSoBsOBQ&ab_channel=npm)
* [Instant Loading: Building offline-first Progressive Web Apps - Google I/O 2016](https://www.youtube.com/watch?v=cmGr0RszHc8&ab_channel=GoogleChromeDevelopers)
* [The disintermediated web - Substack](https://www.youtube.com/watch?v=6jcQoSraHcw&list=PL0CdgOSSGlBYnHAl_DZoy9BWvdVQjNKE2&index=4&ab_channel=NearForm)

