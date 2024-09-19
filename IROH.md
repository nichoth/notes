[via discord](https://discord.com/channels/1161119546170687619/1234486664626442300/1265537846484406334)

----------------------------------------

Unsure if this is the right spot. From [the blog](https://iroh.computer/blog/iroh-and-the-web), it says:

> what you're connecting to needs to be served over DNS and have a working TLS certificate, whomp whooomp. If you want to talk to another machine from your browser, you're pretty much stuck talking to servers only.
and 
> the TLS restrictions keep web applications from innovating beyond the server-client model

This isnt fully true. There is an api called [serverCertificateHashes](https://developer.mozilla.org/en-US/docs/Web/API/WebTransport/WebTransport#servercertificatehashes) which allows browser clients to connect to ip addresses with self-signed certs, *as long as they first pin the hash of the cert before connecting*.

For example, I could give someone a url in a standard format like `https://10.11.12.13:1337/some/path#sha256-of-self-signed-cert-here`, parse out the hash, and the client could then connect over webtransport securely from the browser using self-signed certs (no dns, no letsencrypt/pki), meaning its possible for people to host servers without paying for domains - they just need port forwarding, or to use a solution for hole punching like STUN.

Of course, none of that works if you don't first  exchange the hash of the cert, which means you need to give someone this url out-of-band (perhaps I send you a link on discord) or you need a gateway HTTPS server with a PKI cert to provide a lookup of NodeId -> Cert hash. Despite this limitation, I would assume that the load on the hash lookup server would be much less because its only responsible for sharing the hash rather than performing the full iroh protocol over HTTPS or websockets.

Below is a browser compatibility chart, the api appears supported (see [chrome](https://chromestatus.com/feature/5690646332440576) and the [MDN docs](https://developer.mozilla.org/en-US/docs/Web/API/WebTransport/WebTransport#browser_compatibility) ) by all the browsers that implemented webtransport. Which means all of them except safari (but safari [says they will implement webtransport](https://github.com/WebKit/standards-positions/issues/18) and hopefully that means they will implement serverCertificateHashes too).

Are the iroh devs aware that self-signed certificates and connections to ip addresses (without DNS) are supported in browsers?