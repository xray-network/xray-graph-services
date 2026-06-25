# xray-graph-services

This monorepo contains the services and clients that make up XRAY/Graph.

Each service lives in its own folder with its own setup notes and Docker Compose file. Some services depend on others, so bring them up in dependency order when you are starting a fresh stack.

## Repository Layout

- [cardano-node](cardano-node/README.md)
- [cardano-db-sync](cardano-db-sync/README.md)
- [ogmios](ogmios/README.md)
- [postgres](postgres/README.md)
- [koios-tiny](koios-tiny/README.md)
- [kubo](kubo/README.md)
- [traefik](traefik/README.md)
- [koios-tiny-ts-client](koios-tiny-ts-client/README.md)

## Dependency Order

A typical local bootstrap looks like this:

1. Start [postgres](postgres/README.md).
2. Start [cardano-node](cardano-node/README.md).
3. Start [cardano-db-sync](cardano-db-sync/README.md) and [ogmios](ogmios/README.md).
4. Start [koios-tiny](koios-tiny/README.md).
5. Start [traefik](traefik/README.md) if you want reverse-proxied routing.

Independent services such as [kubo](kubo/README.md) can be started whenever their own configuration is ready.
