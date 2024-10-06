# local first notes

via [the zero discord](https://discord.com/channels/830183651022471199/1246101458928144434/1292526360941563934)

> One thing that isn't widely understood which would be useful to write about is that local-first infra really falls into two camps technically.

> There are in-memory systems and database-backed systems. LiveBlocks, Reflect (our previous product), and yjs are examples of memory-based systems.  Figma also uses a memory-based system for their multiplayer UI. MBS are very fast and suitable for live cursors, but they cannot scale beyond what can fit in memory on a server, so they are really only good for collaborating within a single document.

> DB-backed systems are things like Zero, Replicache, Instant, Electric SQL and so-on. These are inherently slower because the data is being stored in a database at end of day, so they're arent as appropriate for live cursors and drag/drop. But they can scale to much bigger datasets and can be used for the basis for a whole app. Even within Figma there are two realtime systems - one within the doc (in-memory) and one for all the user and file metadata. See https://www.figma.com/blog/livegraph-real-time-data-fetching-at-figma/
