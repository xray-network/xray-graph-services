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
