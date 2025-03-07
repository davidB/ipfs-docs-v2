---
title: Roadmap
description: Learn about the milestones in the IPFS project in order to reach version 1.0.0.
---

# Roadmap: IPFS project requirements to 1.0.0

## Summary

In order for IPFS to reach its maturity state, going from Alpha, to Beta and to v1.0.0, the project will need:

- For its specifications to be 100% complete. This includes the IPFS, libp2p, multiformats and IPLD specs.
- Compliance tests for the specification.
- The golang and JavaScript implementations to be 100% complete and spec compliant.
- A third party implementation of IPFS, fully interoperable with the go and JavaScript versions.
- A release plan and cycle, including a strategy to support specific key releases for longer periods of time (i.e LTS releases vs stable)

Here you will find a comprehensive list of the various challenges and milestones in the IPFS project to reach version 1.0.0. They are not ordered in any way at the moment, merely grouped.

## Sustainability and governance

These are some of the milestones to hit to create a active, sustainable, inclusive and participatory governance model for IPFS.

- [x] Organize IPFS all-hands.
- [ ] Have IPFS lead by a steering working group.
- [x] Define several working groups focused on different parts of the project (e.g community engagement, documentation and education, IPFS in web browsers).
- [ ] Define a release plan and long-term support plan.

## IPFS use cases

These are some use case milestones to drive development.

- [x] Support for file distribution
  - [x] Support for personal file storage, backups, and distribution
  - [x] Support for basic p2p file distribution
  - [x] Support for fast local area network file distribution
- [x] Support for immutable, permanent links to files, websites, data
- [x] Support for mutable links to files, websites, data
- [x] Support for websites and web applications
  - [x] Support for static web applications
  - [x] Support for API based web applications
  - [x] Support for fully dynamic websites entirely on IPFS (eg chat)
- [x] Support for collaborative seeding/pinning
  - [x] basic support for ipfs ref pinning
  - [ ] Cloud ipfs frontend services (cube)
  - [ ] clusters of ipfs nodes (RAID/RAIN)
  - [ ] byzantine clusters (BA)
- [x] Support for browsers
  - [x] js-ipfs-api client inside a tab
  - [x] js-ipfs full node inside a tab
  - [x] browser extension gateway redirects
  - [x] browser extension full node
  - [ ] impl native inside browsers
- [x] Support for versioning and archival
  - [x] archival of files
  - [x] archival of data and databases
  - [ ] commit based versioning
- [x] Support other tools or applications via APIs
  - [x] Support for commandline API usage
  - [x] Support for HTTP API usage
  - [ ] Support for unix sockets RPC API usage
  - [x] Support for embedded, programmatic API usage
  - [x] Support for HTTP gateway

## Performance milestones

These are some basic performance milestones to hit.

- [x] Megabytes / Slow
  - [x] Good enough for small files - MB
  - [x] Good enough for static websites - MB
  - [x] Good enough for distributing webapp code/assets - MB
  - [x] Good enough for images - MB
- [x] Gigabytes
  - [x] Good enough for personal documents - GB
  - [x] Good enough to stream video on the web - GB
  - [x] Good enough for small scientific datasets - GB
  - [x] Good enough for distributing webapp user data - GB
- [ ] Terabytes
  - [x] Good enough for image collections - TB
  - [x] Good enough for small video collections - TB
  - [ ] Good enough for medium scientific datasets - TB
  - [x] Good enough as a package manager (gx) - TB
  - [x] Good enough as a package manager backup (npm-on-ipfs) - TB
  - [ ] Good enough as a package manager replacement (npm-on-ipfs) - TB
  - [x] Good enough to distribute small databases - TB
  - [ ] Good enough for large (single) archives - TB
- [ ] Petabytes
  - [ ] Good enough for large video collections - PB
  - [ ] Good enough for large scientific datasets - PB
  - [ ] Good enough for Backup Archival - TB/PB
  - [ ] Good enough to distribute large databases - PB
- [ ] Exabytes
  - [ ] Good enough for massive archives - EB
  - [ ] Good enough for the entire web - EB
  - [ ] Good enough for top10 websites - EB

## Developer libraries

These are some libraries that must exist to make developers' lives easy. It is critical that making fully dynamic apps on IPFS should be just as easy or easier than traditional systems.

- [x] file importers for basic files
- [x] custom file importer tooling
- [x] ipfs node api bindings
  - [x] ipfs api bindings in Go
  - [x] ipfs api bindings in JS
  - [x] ipfs api bindings in Java
  - [x] ipfs api bindings in Python
  - [x] ipfs api bindings in PHP
  - [x] ipfs api bindings in Ruby
  - [ ] ipfs api bindings in Scala
  - [ ] ipfs api bindings in Rust
  - [ ] ipfs api bindings in Haskell
  - [x] ipfs api bindings in C/C++
  - [ ] ipfs api bindings in Erlang
- [x] full ipfs node implementations
  - [x] go-ipfs - implementation in Go
  - [x] js-ipfs - implementation in JS
- [x] developer libs for cli tools
- [ ] developer libs for desktop apps
- [x] developer libs for webapps
  - [x] js-ipfs-api - js api bindings
- [ ] developer libs for mobile apps
  - [ ] developer libs for iOS
  - [ ] developer libs for Android
- [x] developer libs for node.js apps
  - [x] go-ipfs-dep - module to install go-ipfs
  - [x] ipfsd-ctl - module to control an ipfs daemon
  - [x] js-ipfs-api - js api bindings
- [ ] developer libs for dynamic webapps (in progress)
  - [x] ipfs-log (CRDT)
  - [ ] other "CRDTs on IPFS" libs
  - [x] orbit-db - key-value store and event log
- [ ] developer libs for crypto capabilities
  - [ ] typical sharing models over ipfs
- [ ] developer libs for social networks
  - [ ] POST datastructure
  - [ ] decentralized identity

## Security milestones

- [ ] Network security
  - [x] upgradable transport encryption (multistream)
  - [x] transport encryption: secio (ECDHE)
  - [ ] transport encryption: TLS 1.3 (mainstream crypto)
  - [ ] transport encryption: CurveCP or MinimaLT (djb crypto)
- [ ] Content Security
  - [x] content security: IPLD hash links (authenticated content)
  - [ ] content security: Keychain signed objects
  - [ ] content security: native content encryption
  - [ ] content security: native crypto capabilities
  - [ ] content security: audit
- [ ] Anonymity
  - [ ] transport anonymity: tor support
  - [ ] transport anonymity: i2p support
  - [ ] ship anonymity focused distribution (tor, i2p, no leaking info)
  - [ ] peer and content routing anonymity
  - [ ] anonymity: audit
- [ ] Anticensorship
  - [x] Anticensorship: decentralized, peering content distribution
  - [x] Anticensorship: access based re-distribution
  - [ ] Anticensorship: incentivized distribution
  - [ ] Anticensorship: PKI distribution
  - [ ] Anticensorship: resilience to powerful sybil attacks on routing
  - [ ] Anticensorship: HTTP TLS transport emulation
- [ ] Auditing
  - [ ] Audit: full protocol fuzzer tests
  - [ ] Audit: test with state of the art exploit test suites
  - [ ] Audit: p2p scalability researcher audits
  - [ ] Audit: 3x independent professional security audits of full protocol
  - [ ] Audit: 3x independent professional security audits of implementations

## Network scalability

The scalability of the IPFS protocol depends on careful design of algorithms and models, careful optimization of our implementations, and careful attention to the security properties of the protocols. Reaching high scalability for self-organizing peer-to-peer protocols is HARD, though definitely achievable. We measure scalability in orders of magnitude, as larger thresholds will require revisiting various parts of our codebase.

Please bear in mind that we are currently still implementing major features of the protocols and reaching implementation completion. We have not yet turned our focus towards scalability, thus there are LOTS of low hanging fruit to optimize and likely many scalability bugs to be worked out. The most important part is to make sure all protocols are meant to scale to billions of nodes, and that they make no centralizing assumptions. All protocols we have chosen make no small scale assumptions and are meant to scale well (typically `log(n)`).

Our scalability observations are divided into simulations, real network tests, and production networks.

- [x] Simulations
  - [x] Scalability to 1,000s of nodes
  - [x] Scalability to 10,000s of nodes
  - [x] Scalability to 100,000s of nodes
  - [ ] Scalability to 1,000,000s of nodes
  - [ ] Scalability to 1,000,000,000s of nodes
- [x] Real network tests
  - [x] Scalability to 1,000s of nodes
  - [x] Scalability to 10,000s of nodes
  - [ ] Scalability to 100,000s of nodes
  - [ ] Scalability to 1,000,000s of nodes
  - [ ] Scalability to 1,000,000,000s of nodes
- [x] Production networks
  - [x] Scalability to 1,000s of nodes
  - [x] Scalability to 10,000s of nodes
  - [ ] Scalability to 100,000s of nodes
  - [ ] Scalability to 1,000,000s of nodes
  - [ ] Scalability to 1,000,000,000s of nodes

## Polish level

The polish level achieved defines how much effort has gone into polishing all the corners of the tools, APIs, documentation, and so on. Early on, things will be much more rough as we need to focus on implementation speed over final polish. As we reach completion of the implementations, we turn our focus towards scalability, stability, and security. After that, we focus on end-user polish.

- [x] Polish level: alpha - individuals innovators
- [x] Polish level: alpha - production for early adopters
- [ ] Polish level: beta - production for small orgs (in progress)
- [ ] Polish level: beta - production for large orgs
- [ ] Polish level: 1.0 - production for all


## Multiformats

Multiformats are a set of self-describing protocols/formats for future-proofed or "upgradable systems" (systems that make no assumptions that are likely to break over time).

- [x] multiaddr: protocol design
  - [x] multiaddr: impl in Go
  - [x] multiaddr: impl in JS
  - [x] multiaddr: impl in Java
  - [x] multiaddr: impl in Haskell
  - [x] multiaddr: impl in Python
  - [x] multiaddr: impl in Rust
- [x] multihash: protocol spec
  - [x] multihash: impl in Go
  - [x] multihash: impl in JS
  - [x] multihash: impl in Scala
  - [x] multihash: impl in Java
  - [x] multihash: impl in Clojure
  - [x] multihash: impl in Rust
  - [x] multihash: impl in Haskell
  - [x] multihash: impl in Python
  - [x] multihash: impl in Elixir
  - [x] multihash: impl in Swift
  - [x] multihash: impl in Ruby
- [x] multicodec: protocol spec
  - [x] multicodec: impl in Go
  - [x] multicodec: impl in JS
- [x] multistream: protocol spec
  - [x] multistream: impl in Go
  - [x] multistream: impl in JS
- [x] multibase / baseN: protocol spec
  - [x] multibase / baseN: impl in Go
  - [x] multibase / baseN: impl in JS


## libp2p protocols

The libp2p protocols are the protocol stack for the modular p2p protocols library spun out of IPFS. These form a p2p-first network stack, with no assumptions, self description, and modular interfaces. More at https://github.com/ipfs/specs/tree/master/libp2p

Consult [libp2p requirements here](https://github.com/libp2p/libp2p/blob/master/REQUIREMENTS.md)

## Bitswap

Bitswap is the exchange protocol of IPFS. It simulates a data market.

- [x] Bitswap: Protocol and architecture design
  - [x] Bitswap: protocol spec
  - [x] Bitswap: decision engine
  - [x] Bitswap: strategy: altruist
  - [x] Bitswap: strategy: logistic
  - [x] Bitswap: strategy: programmable
  - [x] Bitswap: support for keys
  - [x] Bitswap: support for paths
  - [ ] Bitswap: support for selectors
  - [ ] Bitswap: hooks for other txns
- [x] Bitswap: impl in Go
  - [x] Bitswap: testing simulator
  - [x] Bitswap: basic exchange
  - [x] Bitswap: bandwidth accounting
  - [x] Bitswap: decision engine
  - [x] Bitswap: strategy: altruist
  - [ ] Bitswap: strategy: logistic
  - [ ] Bitswap: strategy: programmable
  - [x] Bitswap: support for keys
  - [ ] Bitswap: support for paths
  - [ ] Bitswap: support for selectors
  - [ ] Bitswap: hooks for other txns
- [x] Bitswap: impl in JS
  - [x] Bitswap: testing simulator
  - [x] Bitswap: basic exchange
  - [x] Bitswap: bandwidth accounting
  - [x] Bitswap: decision engine
  - [x] Bitswap: strategy: altruist
  - [ ] Bitswap: strategy: logistic
  - [x] Bitswap: strategy: programmable
  - [x] Bitswap: support for keys
  - [ ] Bitswap: support for paths
  - [ ] Bitswap: support for selectors
  - [ ] Bitswap: hooks for other txns
- [x] Bitswap: bssim network simulations
  - [x] Bitswap: bssim: basic in-proc simulation
  - [x] Bitswap: bssim: basic multiproc simulation
  - [ ] Bitswap: bssim: basic multi machine simulation
  - [x] Bitswap: bssim: metrics collection
  - [x] Bitswap: bssim: reporting
  - [x] Bitswap: bssim: pluggable strategies
  - [ ] Bitswap: bssim: strategies config

## IPFS DHT

The IPFS DHT is (today) a Kademlia based DHT implementing several libp2p protocols: peer discovery, peer routing, content routing, and some NAT traversal assistance.

- [x] IPFS DHT: Protocol and architecture design
  - [x] IPFS DHT: protocol spec / messages
  - [x] IPFS DHT: kad queries
  - [x] IPFS DHT: kbucketing
  - [x] IPFS DHT: churn resistance
  - [ ] IPFS DHT: censor resistance
- [x] IPFS DHT: impl in Go
  - [x] IPFS DHT: messages
  - [x] IPFS DHT: kad queries
  - [x] IPFS DHT: kbucketing
  - [x] IPFS DHT: churn resistance
  - [ ] IPFS DHT: censor resistance
- [x] IPFS DHT: impl in JS
  - [x] IPFS DHT: messages
  - [x] IPFS DHT: kad queries
  - [x] IPFS DHT: kbucketing
  - [x] IPFS DHT: churn resistance
  - [ ] IPFS DHT: censor resistance
- [x] IPFS DHT: dhtHell simulations
  - [x] IPFS DHT: dhtHell programmable config
  - [x] IPFS DHT: dhtHell in-proc tests
  - [ ] IPFS DHT: dhtHell multi-proc tests
  - [ ] IPFS DHT: dhtHell multi-machine tests
  - [x] IPFS DHT: dhtHell 1,000 nodes
  - [x] IPFS DHT: dhtHell 10,000 nodes
  - [ ] IPFS DHT: dhtHell 100,000 nodes
  - [ ] IPFS DHT: dhtHell 1,000,000 nodes


## IPFS pub/sub

The IPFS pub/sub service will provide fast delivery and routing for subnets of ipfs nodes. This is critical for dynamic applications. pub/sub (or multicast) will implement: Peer Discovery, Peer Routing, Content Routing, and some NAT Traversal assistance. It fulfills similar roles as the IPFS DHT, but with drastically different performance, security, and scalability guarantees. IPFS Pub/Sub is currently in development.

- [ ] IPFS pub/sub: Protocol and architecture design
  - [ ] IPFS pub/sub: protocol spec / messages
  - [ ] IPFS pub/sub: record spec
  - [x] IPFS pub/sub: one-hop support
  - [ ] IPFS pub/sub: multihop tree forming
  - [ ] IPFS pub/sub: churn resistance
  - [ ] IPFS pub/sub: censor resistance
  - [ ] IPFS pub/sub: topic/channel support
  - [ ] IPFS pub/sub: hierarchical topic/channel support
  - [ ] IPFS pub/sub: authenticated subnets
  - [ ] IPFS pub/sub: private subnets (symmetric)
  - [ ] IPFS pub/sub: private subnets (PKI)
- [ ] IPFS pub/sub: impl in Go
  - [x] IPFS pub/sub: prototyping in Go
- [ ] IPFS pub/sub: impl in JS
  - [x] IPFS pub/sub: prototyping in JS
- [ ] IPFS pub/sub: pssim simulations
  - [ ] IPFS pub/sub: pssim programmable config
  - [ ] IPFS pub/sub: pssim in-proc tests
  - [ ] IPFS pub/sub: pssim multi-proc tests
  - [ ] IPFS pub/sub: pssim multi-machine tests
  - [ ] IPFS pub/sub: pssim 1,000 nodes
  - [ ] IPFS pub/sub: pssim 10,000 nodes
  - [ ] IPFS pub/sub: pssim 100,000 nodes
  - [ ] IPFS pub/sub: pssim 1,000,000 nodes

## IPLD

IPLD is the core format for data on IPFS. More at https://github.com/ipfs/specs/tree/master/ipld

- [x] ipld v0 protobuf: spec
  - [x] ipld v0 protobuf: impl in go
  - [x] ipld v0 protobuf: impl in js
- [x] ipld: spec
  - [x] ipld: Linking
  - [x] ipld: Pathing
  - [ ] ipld: Selector
  - [ ] ipld: Query
  - [x] ipld: v0 compat
  - [x] ipld: cbor serialization
  - [x] ipld: links and resolving
  - [x] ipld: streaming support
- [x] ipld: impl in Go
  - [x] ipld: Linking
  - [x] ipld: Pathing
  - [ ] ipld: Selector
  - [ ] ipld: Query
  - [x] ipld: v0 compat
  - [x] ipld: cbor serialization
  - [x] ipld: links and resolving
  - [x] ipld: streaming support
- [x] ipld: impl in JS
  - [x] ipld: Linking
  - [x] ipld: Pathing
  - [ ] ipld: Selector
  - [ ] ipld: Query
  - [x] ipld: v0 compat
  - [x] ipld: cbor serialization
  - [x] ipld: links and resolving
  - [ ] ipld: streaming support
- [ ] ipld: website
  - [ ] ipld: website: front page
  - [ ] ipld: website: spec
  - [ ] ipld: website: about
  - [ ] ipld: website: playground
    - [ ] ipld: website: playground spec
    - [ ] ipld: website: playground impl

## IPLD data structures and importers

IPLD data structures and importers are various data structures and programs that covert data or files from other native representations to and from IPLD graphs. Think of these as both the graph representation datastructs, and conversion codecs.

- [x] unixfs for unix/posix files
  - [x] unixfs spec
    - [x] unixfs file
    - [x] unixfs file sharding
    - [x] unixfs file trickledag
    - [x] unixfs dir
    - [ ] unixfs dir sharding
    - [x] unixfs metadata
  - [x] unixfs impl in Go
    - [x] unixfs file
    - [x] unixfs file sharding
    - [x] unixfs file trickledag
    - [x] unixfs dir
    - [x] unixfs dir sharding
    - [x] unixfs metadata
  - [x] unixfs impl in JS
    - [x] unixfs file
    - [x] unixfs file sharding
    - [x] unixfs file trickledag
    - [x] unixfs dir
    - [x] unixfs dir sharding
    - [x] unixfs metadata
- [x] archives spec
  - [x] tar
  - [ ] zip
  - [ ] rar
- [ ] keychain spec
  - [ ] keychain: keys
  - [ ] keychain: sigs
  - [ ] keychain: caps
  - [ ] keychain: proofs

## IPFS repo

More at https://github.com/ipfs/specs and  https://github.com/ipfs/fs-repo-migrations

- [x] IPFS repo spec
  - [x] IPFS repo impl in Go
  - [x] IPFS repo impl in JS node
  - [x] IPFS repo impl in JS browser
- [x] IPFS fs-repo spec
  - [x] IPFS fs-repo v0
    - [x] IPFS fs-repo datastore (blocks and metadata)
    - [x] IPFS fs-repo config file
    - [x] IPFS fs-repo lock file
    - [x] IPFS fs-repo logs dir
  - [x] IPFS fs-repo v1
    - [x] IPFS fs-repo version file
    - [x] IPFS fs-repo api file
    - [x] IPFS fs-repo blocks (data)
    - [x] IPFS fs-repo datastore (metadata)
  - [x] IPFS fs-repo v2
    - [x] IPFS fs-repo ipld pinset
  - [x] IPFS fs-repo impl in Go
  - [x] IPFS fs-repo impl in JS node
  - [x] IPFS fs-repo impl in JS browser
  - [x] IPFS fs-repo-migrations
    - [x] IPFS fs-repo-migrations 0-to-1
    - [x] IPFS fs-repo-migrations 1-to-2
    - [x] IPFS fs-repo-migrations 2-to-3

## IPFS protocol and architecture

- [x] IPFS architecture: macro protocol architecture
- [x] IPFS architecture: futureproofing and self-description (multis)
- [x] IPFS architecture: networking
  - [x] IPFS architecture: encrypted and authenticated connectivity
  - [x] IPFS architecture: peer and content routing
  - [x] IPFS architecture: NAT traversal
  - [x] IPFS architecture: line and pkt switching relay
  - [x] IPFS architecture: abstracting and extracting libp2p
  - [x] IPFS architecture: basic private networks (symmetric encryption)
  - [ ] IPFS architecture: advanced private networks (PKI)
- [x] IPFS architecture: merkle-linked graph and IPLD
  - [x] IPFS architecture: pathing model for fs and web
  - [x] IPFS architecture: selectors for graph traversals
- [x] IPFS architecture: addressing
  - [x] IPFS architecture: content addressing and resolution
  - [x] IPFS architecture: key addressing and resolution
  - [x] IPFS architecture: other resolver addressing and resolution
- [x] IPFS architecture: node data sync model
  - [x] IPFS architecture: ref pull resolution and retrieval
  - [ ] IPFS architecture: ref push
  - [x] IPFS architecture: ref pinning
  - [ ] IPFS architecture: peer-to-peer RPC auth
- [x] IPFS architecture: projection of protocol to programs
  - [x] IPFS architecture: program model
  - [x] IPFS architecture: service design
  - [x] IPFS architecture: tool design
  - [x] IPFS architecture: core API design
    - [x] IPFS architecture: CLI API design
    - [x] IPFS architecture: HTTP API design
    - [ ] IPFS architecture: RPC API design
- [x] IPFS architecture: distribution of programs
- [x] IPFS architecture: WebUI design
- [x] IPFS architecture: app designs
- [ ] IPFS architecture: programmable policy hooks
  - [ ] IPFS architecture: bitswap strategies and trading
  - [ ] IPFS architecture: data advertising and serving
  - [ ] IPFS architecture: social network
  - [x] IPFS architecture: blocklists design
    - [ ] IPFS architecture: blocklist support in gateway
    - [ ] IPFS architecture: blocklist support in net
    - [ ] IPFS architecture: scalable blocklist (bloom)
- [ ] IPFS architecture: clustering
  - [ ] IPFS architecture: cluster RAID/RAIN modes
  - [ ] IPFS architecture: cluster consensus

## Go implementation of IPFS

The go-ipfs effort is the Go implementation of IPFS. It is meant to run as a command-line tool, as a background service, as a programmatic embedded node, through an RPC API, and to be used as part of other tools. go-ipfs is the reference implementation of IPFS. It includes the HTTP-to-IPFS gateway implementation. More at https://github.com/ipfs/go-ipfs

- [x] go-ipfs ipfs node components
  - [x] go-ipfs multi protocols
  - [x] go-ipfs component: repo
  - [x] go-ipfs component: networking (libp2p)
  - [x] go-ipfs component: bitswap
  - [x] go-ipfs component: dag / ipld
  - [x] go-ipfs component: pinning
  - [x] go-ipfs component: block api
  - [x] go-ipfs component: object api
  - [x] go-ipfs component: files api
  - [x] go-ipfs component: daemon
  - [x] go-ipfs component: data importing
  - [x] go-ipfs component: gateway
  - [x] go-ipfs component: http api
- [x] go-ipfs ipfs node api
  - [x] go-ipfs core api impl
    - [x] go-ipfs core api: version
    - [x] go-ipfs core api: daemon
    - [x] go-ipfs core api: id
    - [x] go-ipfs core api: block
    - [x] go-ipfs core api: object
    - [x] go-ipfs core api: refs
    - [x] go-ipfs core api: repo
    - [x] go-ipfs core api: pin
    - [x] go-ipfs core api: log
  - [x] go-ipfs ext api impl
    - [x] go-ipfs ext api: name (ipns)
    - [x] go-ipfs ext api: dns
    - [x] go-ipfs ext api: tar
    - [ ] go-ipfs ext api: tour
    - [x] go-ipfs ext api: files
    - [x] go-ipfs ext api: stat
    - [x] go-ipfs ext api: mount
    - [x] go-ipfs ext api: bootstrap
    - [x] go-ipfs ext api: bitswap
  - [x] go-ipfs tool api impl
    - [x] go-ipfs tool api: init
    - [x] go-ipfs tool api: config
    - [x] go-ipfs tool api: update
    - [x] go-ipfs tool api: commands
  - [x] go-ipfs net api impl
    - [x] go-ipfs net api: ping
    - [x] go-ipfs net api: dht
    - [x] go-ipfs net api: swarm
    - [ ] go-ipfs net api: records
- [x] go-ipfs cli api impl
  - [x] go-ipfs cli codecs
- [x] go-ipfs http api impl
  - [x] go-ipfs http api: streaming
  - [x] go-ipfs http api: multipart

## JavaScript implementation of IPFS

The js-ipfs effort is the JavaScript implementation of IPFS. It is meant to run on both node.js and today's regular web browsers. More at https://github.com/ipfs/js-ipfs

- [x] js-ipfs ipfs node components
  - [x] js-ipfs multi protocols
  - [x] js-ipfs component: repo
  - [x] js-ipfs component: networking (libp2p)
  - [x] js-ipfs component: bitswap
  - [x] js-ipfs component: dag/IPLD
  - [x] js-ipfs component: pinning
  - [x] js-ipfs component: block API
  - [x] js-ipfs component: object API
  - [x] js-ipfs component: files API
  - [x] js-ipfs component: daemon
  - [x] js-ipfs component: data importing
  - [x] js-ipfs component: http API
- [ ] js-ipfs ipfs node api
  - [x] js-ipfs core api impl
    - [x] js-ipfs core api: version
    - [x] js-ipfs core api: daemon
    - [x] js-ipfs core api: id
    - [x] js-ipfs core api: block
    - [x] js-ipfs core api: object
    - [ ] js-ipfs core api: refs
    - [x] js-ipfs core api: repo
    - [x] js-ipfs core api: pin
    - [ ] js-ipfs core api: log
  - [ ] js-ipfs ext api impl
    - [ ] js-ipfs ext api: name (ipns)
    - [ ] js-ipfs ext api: dns
    - [ ] js-ipfs ext api: tar
    - [x] js-ipfs ext api: files
    - [ ] js-ipfs ext api: stat
    - [ ] js-ipfs ext api: mount
    - [x] js-ipfs ext api: bootstrap
    - [x] js-ipfs ext api: bitswap
  - [x] js-ipfs tool api impl
    - [x] js-ipfs tool api: init
    - [x] js-ipfs tool api: config
    - [ ] js-ipfs tool api: update
    - [x] js-ipfs tool api: commands
  - [ ] js-ipfs net api impl
    - [x] js-ipfs net api: ping
    - [ ] js-ipfs net api: dht
    - [x] js-ipfs net api: swarm
    - [ ] js-ipfs net api: records
- [x] js-ipfs cli api impl
- [x] js-ipfs http api impl
  - [x] js-ipfs http api: streaming
  - [x] js-ipfs http api: multipart

## IPFS directly in browsers

As a protocol for the web, the ultimate goal of IPFS is to run directly in browsers. We are achieving this through a four-step plan:

- (1) Implement IPFS in any language, and use a js-ipfs-api library to delegate commands to an IPFS API (e.g. go-ipfs running on localhost). This already works today, and many applications already exist leveraging IPFS in the browser this way.
- (2) Implement IPFS in javascript, and use js-ipfs directly in the browser tab. This is in progress today.
- (3) Build browser extensions that use IPFS to serve IPFS URIs and expose ipfs to the browser tab. This can be done using go-ipfs (API on localhost) or ideally a bundled js-ipfs. This is in progress today. The firefox extension already has 400+ daily users.
- (4) Finally, submit patches to the major browsers adding IPFS support.

We have finished step (1). We are currently working on steps (2) and (3). 

- [x] IPFS API used in a browser tab
  - [x] go-ipfs implementation
  - [x] js-ipfs-api client library
  - [x] use background go-ipfs node (localhost or elsewhere)
- [x] IPFS protocol running in a browser tab, in JS
  - [x] js-libp2p implementation
  - [x] js-ipfs implementation
  - [x] libp2p.js browser library
  - [x] ipfs.js browser library
- [x] IPFS running with a browser extension
  - [x] go-ipfs implementation
  - [x] js-ipfs implementation
  - [x] Firefox extension
    - [x] use background go-ipfs node
    - [ ] easy install of go-ipfs node
    - [x] bundling of js-ipfs node
    - [x] URL rewriting
    - [x] node management
    - [x] API configuration
    - [ ] simple UX for users
    - [ ] expose IPFS and p2p in the browser window
  - [x] Chrome extension
    - [x] use background go-ipfs node
    - [ ] easy install of go-ipfs node
    - [x] bundling of js-ipfs node
    - [x] url rewriting
    - [ ] node management
    - [ ] api configuration
    - [ ] simple UX for users
    - [x] expose IPFS and p2p in the browser window
- [ ] IPFS running natively in a browser
  - [x] go-ipfs implementation (for Chrome or Firefox)
    - [ ] go-ipfs static lib (for Chrome or Firefox)
  - [x] js-ipfs implementation (for Chrome or Firefox)
  - [ ] rust-ipfs implementation (for Servo)
  - [ ] Chromium patches adding IPFS support
  - [ ] Firefox patches adding IPFS support
  - [ ] Servo patches adding IPFS support
  - [ ] Safari patches adding IPFS support


## IPFS node management Console (WebUI)

We have an IPFS node "management console" GUI, delivered as a distributed webapp (dapp). This shows information about an IPFS node, and allows issuing some commands. The WebUI is entirely hosted and distributed through IPFS itself, demonstrating dynamic web applications on IPFS. More at https://github.com/ipfs/webui

- [x] webui console architecture
  - [x] R/W privileged API route (:5001)
    - [x] Security: Origin and CORS
    - [x] Security: exposed only locally
    - [ ] Security: token based access
  - [x] distributed through IPFS itself
  - [x] accessed through http-to-ipfs gateway
- [x] webui console v0
  - [x] webapp design
  - [x] basic node info
  - [x] peer map (3D earth)
  - [x] ipfs dag explorer
  - [x] ipfs file viewer
    - [x] listing all files
    - [x] adding files (+ drag and drop)
  - [x] tail logs (json)
  - [x] view & edit config (json)
- [x] webui console v1
  - [x] webapp redesign
  - [x] peer map (flat and 3D)
  - [x] new dag explorer
  - [x] new file explorer
    - [x] file navigation
    - [x] drag and drop support
    - [x] file previews


## HTTP-to-IPFS gateway

In order to ease the adoption and deployment of IPFS, we have HTTP-to-IPFS gateways. This means two related things: (a) implementation of an HTTP-to-IPFS gateway server (currently part of go-ipfs), and (b) a globally accessible service Protocol Labs runs for the community. All of the official IPFS websites are now self-hosted directly on IPFS.

- [x] HTTP gateway implementation (in go-ipfs)
  - [x] HTTP gateway file listing
  - [x] HTTP gateway /ipfs route for files
  - [x] HTTP gateway /ipns route for names
  - [ ] HTTP gateway /ipfs POST writes
  - [ ] HTTP gateway /ipns PUT/POST writes
  - [x] HTTP gateway CORS and headers support
- [x] HTTP gateway service (ipfs.io)
  - [x] HTTP gateway service: solarnet vps infrastructure
  - [x] HTTP gateway service: DNS architecture
    - [x] HTTP gateway service DNS: deployed at ipfs.io
    - [x] HTTP gateway service DNS: dnslink, CNAME, A support
    - [ ] HTTP gateway service DNS: zone automation
    - [ ] HTTP gateway service DNS: TLD redundancy
  - [x] HTTP gateway service: nginx frontend
    - [x] HTTP gateway service: backend fallbacks
    - [x] HTTP gateway service: nginx blocklists (dmca)
    - [ ] HTTP gateway service: rate limiting
  - [x] HTTP gateway service devops
    - [x] HTTP gateway service Devops: containers
    - [x] HTTP gateway service Devops: automated deployments
    - [x] HTTP gateway service Devops: logging
    - [x] HTTP gateway service Devops: event monitoring
    - [x] HTTP gateway service Devops: status alerts
    - [ ] HTTP gateway service Devops: status webpage (status.ipfs.io)
    - [ ] HTTP gateway service Devops: chaos monkey
- [x] HTTP gateway self-hosting
  - [x] HTTP gateway self-hosting: ipfs.io project website
  - [x] HTTP gateway self-hosting: dist.ipfs.io
  - [x] HTTP gateway self-hosting: blog.ipfs.io
  - [x] HTTP gateway self-hosting: refs.ipfs.io

## IPFS distributions

"IPFS distributions" means the distribution model for IPFS project programs. This means a repository of pages, source, binaries, and links for all programs officially distributed by the project.

- [x] IPFS distributions: architecture
- [ ] IPFS distributions: security
  - [x] IPFS distributions: TLS cert for HTTP site
  - [ ] IPFS distributions: code signing
    - [x] IPFS distributions: code signing source
    - [x] IPFS distributions: code signing protocol
    - [x] IPFS distributions: code signing team yubikeys
- [x] IPFS distributions: website
  - [x] IPFS distributions: website design
  - [x] IPFS distributions: website landing page
  - [x] IPFS distributions: website program listings
  - [x] IPFS distributions: website domain (dist.ipfs.io)
  - [ ] IPFS distributions: website localization
- [x] IPFS distributions: tools
  - [x] IPFS distributions: go-ipfs
  - [x] IPFS distributions: ipfs-update
  - [x] IPFS distributions: ipget
  - [x] IPFS distributions: fs-repo-migrations
  - [x] IPFS distributions: gx, gx-go
  - [ ] IPFS distributions: station
  - [ ] IPFS distributions: webui

## Security

- [ ] Create a bug bounty program for IPFS
- [ ] Have IPFS go and js implementations be fully Audited
- [ ] Create a Security Working Group
- [ ] Create a responsible disclosure program

## IPFS blog and newsletter

In order to keep the community updated, we run a blog. This blog is distributed through IPFS itself, and through an email newsletter.

- [x] ipfs blog
  - [x] blog design
  - [x] distribute through ipfs
  - [x] blog.ipfs.io domain
  - [ ] use POST datastructure
- [x] weekly/newsletter
  - [x] establish newsletter process
  - [x] highlight contributions and contributors
  - [x] post to the blog
- [x] email subscription
  - [x] use tinyletter
  - [x] post weekly
  - [ ] post blog
