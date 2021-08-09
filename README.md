

# The `StreamingFast` platform

<img src="https://www.dfuse.io/hubfs/dfuse-website/dfuse-logo2.svg" align="right"
     alt="StreamingFast logo" width="315" height="100">
&nbsp;&nbsp;&nbsp;&nbsp; `StreamingFast` is an Open Source suite of products that enables low-latency, real-time processing
of blockchain data streams, allows for massively parallelizable operations over historical
data, and provides the robustness and reliability required by the most demanding loads.

## Features

It is protocol-aware, supports multiple chain protocols and can be
used to build higher-order blockchain data services.

`StreamingFast` products include a powerful real-time search engine
([StreamingFast Search](https://github.com/streamingfast/search)), mempool
management technologies (StreamingFast Lifecycle), historical state services
and several specialized indexers.


## Installation

Each blockchain protocol has its own installation method. See section below.


## Protocols

Here's a list of blockchain protocols that integrate with the StreamingFast stack:

* [**EOSIO on StreamingFast**](https://github.com/streamingfast/sf-eosio)
* [**Ethereum on StreamingFast**](https://github.com/streamingfast/sf-ethereum)


## Overview

The StreamingFast platform is composed of multiple open-source repositories.  Here is a breakdown.

Top-tier products / solutions:

* [StreamingFast Search](https://github.com/streamingfast/search), distributed, real-time, fork-aware, general purpose search engine.
* [StreamingFast FluxDB](https://github.com/streamingfast/sf-eosio/tree/develop/fluxdb), state snapshotting service for EOSIO.
* [EOSIO Websocket interface](https://github.com/streamingfast/sf-eosio/tree/develop/eosws)
* [EOSIO Push Guarantee](https://github.com/streamingfast/sf-eosio/tree/develop/eosws)
* [EOSIO Transaction Lifecycle](https://github.com/streamingfast/sf-eosio/tree/develop/eosws)
* [EOSIO Blockchain node manager](https://github.com/streamingfast/manageos)
* [EOSIO Point-in-time recovery backup solution](https://github.com/eoscanada/pitreos) (for EOSIO state & blocks files)
* Ethereum Transaction Lifecycle service, coming as Open Source soon
* Ethereum Historical State service, coming as Open Source soon
* Ethereum Speculative EVM execution engine, coming as Open Source soon

Common interfaces:
* gRPC [service definitions](https://github.com/streamingfast/service-definitions) and common Protobuf data models.
* Common [GraphQL service](https://github.com/streamingfast/dgraphql) (see protocol-specific resolvers and schemas)
* [REST + WS for EOSIO](https://github.com/streamingfast/sf-eosio/tree/develop/eosws)

Second-tier service mesh:
* [merger](https://github.com/streamingfast/merger), collecting all forks info, for high-availability deployments.
* [relayer](https://github.com/streamingfast/relayer), streaming blocks relayer, for high-availaibility deployments.
* [block metadata service](https://github.com/streamingfast/blockmeta), offers fast access to the state of the chain's blocks, aware of on-going forks, finality, etc.

Documentation:
* [The StreamingFast docs](https://github.com/streamingfast/docs) rendered at https://docs.dfuse.io

Building blocks:
* The [`bstream` blocks & transactions streaming library](https://github.com/streamingfast/bstream)
* The [`kvdb` key-value storage abstraction](https://github.com/streamingfast/kvdb)

More general purpose Go tooling provided by `StreamingFast`:
* [Errors management library](https://github.com/streamingfast/derr)
* [Object storage abstraction](https://github.com/streamingfast/dstore)
* [Binary file packer](https://github.com/streamingfast/dbin)
* [gRPC tools](https://github.com/streamingfast/dgrpc)
* [Authentication Plugins Interfaces](https://github.com/streamingfast/dauth)
* [Consumption & Metering Plugins Interface](https://github.com/streamingfast/dmetering)
* [Mesh Service Discovery library](https://github.com/streamingfast/dmesh) (used by Search)
* [Simple obfuscation library](https://github.com/streamingfast/opaque)

## License

All `StreamingFast` components are generally **Apache 2.0** licensed.  See repositories for details.
