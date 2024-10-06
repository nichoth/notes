# local first notes

via [the zero discord](https://discord.com/channels/830183651022471199/1246101458928144434/1292526360941563934)

> One thing that isn't widely understood which would be useful to write about is that local-first infra really falls into two camps technically.

> There are in-memory systems and database-backed systems. LiveBlocks, Reflect (our previous product), and yjs are examples of memory-based systems.  Figma also uses a memory-based system for their multiplayer UI. MBS are very fast and suitable for live cursors, but they cannot scale beyond what can fit in memory on a server, so they are really only good for collaborating within a single document.

> DB-backed systems are things like Zero, Replicache, Instant, Electric SQL and so-on. These are inherently slower because the data is being stored in a database at end of day, so they're arent as appropriate for live cursors and drag/drop. But they can scale to much bigger datasets and can be used for the basis for a whole app. Even within Figma there are two realtime systems - one within the doc (in-memory) and one for all the user and file metadata. See https://www.figma.com/blog/livegraph-real-time-data-fetching-at-figma/

> So Zero vs LB the principle difference is that Zero can have way more data in it. Zero can store tens of GB at launch, eventually TB and LB is limited to something like 64MB. But that's not really a defficiency of LB is just not meant for the same thing.

> The other big division you can make in the space is "databases vs sync engines". Zero, Electric, PowerSync are examples of sync engines. They are not themselves an authoritative database, they sit in from of some other AD. At alpha zero will have support for only PG, but it can be extended to support most common database systems and eventually even custom backends.

> Instant, Triplit are examples of database. They have a sync engine inside but they are also the authoritative backend database. This design is easier to build and more tightly integrated, so setup can be a little nicer and easier for users. But it means you have to rely on a new backend database and integration with other common tools in the ecosystem is harder.
