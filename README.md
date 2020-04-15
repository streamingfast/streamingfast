# The `dfuse` data stack

dfuse is an open source suite of products that handles real-time flows
of data as well as massively parallelizable operations of blockchain
data.

It is protocol-aware, supports multiple chain protocols and can be
used to build higher-order blockchain data services.

dfuse products include a powerful real-time search engine
([dfuse Search](https://github.com/dfuse-io/search), mempool
management technologies (dfuse Lifecycle), historical state services
and several specialized indexers.


## Installation

Reach out for binaries in the different
[protocols-specific repositories](#protocols).


## Protocols

Here's a list of blockchain protocols that integrate with the dfuse stack:

* [*dfuse for EOSIO*](https://github.com/dfuse-io/dfuse-eosio)
* *dfuse for Ethereum*, open sources soon!


## Overview

Top-tier products:

* [dfuse Search](https://github.com/dfuse-io/search), distributed, real-time, fork-aware, general purpose search engine.
* [dfuse FluxDB](https://github.com/dfuse-io/dfuse-eosio/tree/develop/fluxdb), state snapshotting service for EOSIO.
* [EOSIO Websocket interface](https://github.com/dfuse-io/dfuse-eosio/tree/develop/eosws)
* [EOSIO Push Guarantee](https://github.com/dfuse-io/dfuse-eosio/tree/develop/eosws)
* [EOSIO Transaction Lifecycle](https://github.com/dfuse-io/dfuse-eosio/tree/develop/eosws)
* Ethereum Transaction Lifecycle service, open sources soon
* Ethereum Historical State service, open sources soon
* Ethereum Speculative EVM execution engine, open sources soon

Common interfaces:
* gRPC [service-definitions](https://github.com/dfuse-io/service-definitions) and common data models.
* [GraphQL service](https://github.com/dfuse-io/dgraphql) (see protocol-specific resolvers and schemas)
* [REST API](https://github.com/dfuse-io/dfuse-eosio/tree/develop/eosws)

Second-tier service mesh:
* [merger](https://github.com/dfuse-io/merger), collecting all forks info, for high-availability deployments.
* [relayer](https://github.com/dfuse-io/relayer), streaming blocks relayer, for high-availaibility deployments.
* [block metadata service](https://github.com/dfuse-io/blockmeta),


Building blocks:

* The [`bstream` blocks & transactions streaming library](https://github.com/dfuse-io/bstream)
* The [`kvdb` key-value storage abstraction](https://github.com/dfuse-io/kvdb)



## Managed deployments

https://dfuse.io Platform Inc. offers professionnally hosted
deployments of dfuse, for public and private networks.

Thanks for supporting us.
