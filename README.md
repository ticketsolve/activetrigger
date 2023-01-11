# ActiveTrigger

ActiveTrigger is a trigger-based callback system.

The idea is that Rails callbacks, at scale, require a significant amount of effort in order to catch all events (primarily, direct SQL execution); by basing the callback system on database triggers, maintenance becomes considerably easier, and fundamentally "inescapable"!

## Development

We've been using this in production for a very long time, with a MySQL backend; the large step to open source it, is to integrate it in a generic way with Rails (we use custom hooks), which we're currently investigating.

We intend to start supporting, from the beginning, MySQL and PostgreSQL.
