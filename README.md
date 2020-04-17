

# The `dfuse` platform

<img src="https://www.dfuse.io/hubfs/dfuse-website/dfuse-logo2.svg" align="right"
     alt="dfuse logo" width="315" height="100">
&nbsp;&nbsp;&nbsp;&nbsp; `dfuse` is an Open Source suite of products that enables low-latency, real-time processing
of blockchain data streams, allows for massively parallelizable operations over historical
data, and provides the robustness and reliability required by the most demanding loads.

## Features

It is protocol-aware, supports multiple chain protocols and can be
used to build higher-order blockchain data services.

`dfuse` products include a powerful real-time search engine
([dfuse Search](https://github.com/dfuse-io/search)), mempool
management technologies (dfuse Lifecycle), historical state services
and several specialized indexers.


## Installation

Each blockchain protocol has its own installation method. See section below.


## Protocols

Here's a list of blockchain protocols that integrate with the dfuse stack:

* [**dfuse for EOSIO**](https://github.com/dfuse-io/dfuse-eosio)
* **dfuse for Ethereum**, coming as Open Source soon!


## Overview

The dfuse platform is composed of multiple open-source repositories.  Here is a breakdown.

Top-tier products / solutions:

* [dfuse Search](https://github.com/dfuse-io/search), distributed, real-time, fork-aware, general purpose search engine.
* [dfuse FluxDB](https://github.com/dfuse-io/dfuse-eosio/tree/develop/fluxdb), state snapshotting service for EOSIO.
* [EOSIO Websocket interface](https://github.com/dfuse-io/dfuse-eosio/tree/develop/eosws)
* [EOSIO Push Guarantee](https://github.com/dfuse-io/dfuse-eosio/tree/develop/eosws)
* [EOSIO Transaction Lifecycle](https://github.com/dfuse-io/dfuse-eosio/tree/develop/eosws)
* [EOSIO Blockchain node manager](https://github.com/dfuse-io/manageos)
* [EOSIO Point-in-time recovery backup solution](https://github.com/eoscanada/pitreos) (for EOSIO state & blocks files)
* Ethereum Transaction Lifecycle service, coming as Open Source soon
* Ethereum Historical State service, coming as Open Source soon
* Ethereum Speculative EVM execution engine, coming as Open Source soon

Common interfaces:
* gRPC [service definitions](https://github.com/dfuse-io/service-definitions) and common Protobuf data models.
* Common [GraphQL service](https://github.com/dfuse-io/dgraphql) (see protocol-specific resolvers and schemas)
* [REST + WS for EOSIO](https://github.com/dfuse-io/dfuse-eosio/tree/develop/eosws)

Second-tier service mesh:
* [merger](https://github.com/dfuse-io/merger), collecting all forks info, for high-availability deployments.
* [relayer](https://github.com/dfuse-io/relayer), streaming blocks relayer, for high-availaibility deployments.
* [block metadata service](https://github.com/dfuse-io/blockmeta), offers fast access to the state of the chain's blocks, aware of on-going forks, finality, etc.

Documentation:
* [The dfuse docs](https://github.com/dfuse-io/docs) rendered at https://docs.dfuse.io

Building blocks:
* The [`bstream` blocks & transactions streaming library](https://github.com/dfuse-io/bstream)
* The [`kvdb` key-value storage abstraction](https://github.com/dfuse-io/kvdb)

More general purpose Go tooling provided by `dfuse`:
* [Errors management library](https://github.com/dfuse-io/derr)
* [Object storage abstraction](https://github.com/dfuse-io/dstore)
* [Binary file packer](https://github.com/dfuse-io/dbin)
* [gRPC tools](https://github.com/dfuse-io/dgrpc)
* [Authentication Plugins Interfaces](https://github.com/dfuse-io/dauth)
* [Consumption & Metering Plugins Interface](https://github.com/dfuse-io/dmetering)
* [Mesh Service Discovery library](https://github.com/dfuse-io/dmesh) (used by Search)
* [Simple obfuscation library](https://github.com/dfuse-io/opaque)


## Managed deployments

[dfuse Platform Inc.](https://dfuse.io) offers professionally hosted
deployments of dfuse, for public and private networks.

Thanks for supporting us.

## License

All `dfuse` components are generally **Apache 2.0** licensed.  See repositories for details.
