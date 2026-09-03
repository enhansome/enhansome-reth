# awesome-reth with stars

**A list of awesome Reth-related resources**.

* [Repository](https://github.com/paradigmxyz/reth) ⭐ 5,764 | 🐛 265 | 🌐 Rust | 📅 2026-09-03
* [User Book](https://reth.rs)

[Follow me](https://twitter.com/secjack_) for live updates as I usually retweet whatever I find. Alternatively, feel free to contribute to this list by opening a PR!

## Audits

* [Sigma Prime](https://github.com/paradigmxyz/reth/blob/0a49d47dc33058cafe5d3decfce85a3a81de62f9/Sigma_Prime_Paradigm_Reth_Security_Assessment_Report_v1_0.pdf) ⭐ 5,764 | 🐛 265 | 🌐 Rust | 📅 2026-09-03

## Development Tools

* [ethers-reth](https://github.com/SorellaLabs/ethers-reth) ⭐ 270 | 🐛 2 | 🌐 Rust | 📅 2023-10-18, an [Ethers-rs](https://ethers.rs)-aware middleware by [Sorella Labs](https://github.com/SorellaLabs) for accessing Reth state directly ([Tweet](https://x.com/0xvanbeethoven/status/1668434735281090560))
* [Reth Alphanet](https://github.com/paradigmxyz/alphanet) ⚠️ Archived, OP-Stack compatible testnet rollup explicitly designed for Ethereum R\&D ([blog post](https://www.paradigm.xyz/2024/04/reth-alphanet), [Tweet](https://x.com/gakonst/status/1779892069169008709))

## MEV

* [NodeDB](https://github.com/Zacholme7/NodeDB) ⭐ 46 | 🐛 0 | 🌐 Rust | 📅 2025-05-26, updates [revm](https://github.com/bluealloy/revm) ⭐ 2,225 | 🐛 92 | 🌐 Rust | 📅 2026-09-03's database directly from Reth's database
* [reth-private-transaction](https://github.com/Quertyy/reth-private-transaction) ⭐ 40 | 🐛 0 | 🌐 Rust | 📅 2024-12-15, `eth_sendPrivateRawTransaction` implementation that punches straight through to the top three block builders
* [rethdb-dexsync](https://github.com/cakevm/rethdb-dexsync) ⭐ 29 | 🐛 0 | 🌐 Rust | 📅 2024-10-20, retrieve CFMM pool state directly from Reth's database
* [alloy-reth-provider](https://github.com/cakevm/alloy-reth-provider) ⭐ 11 | 🐛 0 | 🌐 Rust | 📅 2025-07-16, retrieve state from a remote node via Alloy

## Execution Extensions (ExExes)

An [Execution Extension (ExEx)](https://www.paradigm.xyz/2024/05/reth-exex) is code that runs in-process with Reth that has access to *reorg-aware* chain state. Consult [the official documentation](https://reth.rs/developers/exex/exex.html) for more details.

* [loom-exex](https://github.com/dexloom/loom/tree/main/bin/loom_exex) ⭐ 331 | 🐛 0 | 🌐 Rust | 📅 2025-07-26, an ExEx for backrunning (part of the larger [loom](https://github.com/dexloom/loom) ⭐ 331 | 🐛 0 | 🌐 Rust | 📅 2025-07-26 project)
* [reth-exex-examples](https://github.com/paradigmxyz/reth-exex-examples) ⭐ 165 | 🐛 13 | 🌐 Rust | 📅 2026-04-29, an official repository of example ExEx implementations
* [shadow-reth](https://github.com/shadow-hq/shadow-reth) ⭐ 111 | 🐛 3 | 🌐 Rust | 📅 2024-12-16, an implementation of the [Shadow RPC](https://docs.shadow.xyz/product-guide/shadow-rpc) as an ExEx ([blog post](https://blog.shadow.xyz/shadow-reth))
* [exex-indexer](https://github.com/gibz104/exex-indexer) ⭐ 34 | 🐛 0 | 🌐 Rust | 📅 2025-11-18, an ExEx providing blockchain indexing
* [flare](https://github.com/rauljordan/flare) ⭐ 19 | 🐛 0 | 🌐 Rust | 📅 2024-05-05, an ExEx that indexes [Arbitrum](https://arbitrum.io) sequencer batches ([Tweet](https://mobile.x.com/rauljordaneth/status/1787252292250485231))
* [reth-exex-plugin](https://github.com/0xurb/reth-exex-plugin) ⭐ 16 | 🐛 0 | 🌐 Rust | 📅 2024-10-12, an ExEx facilitating dynamic code injection via shared libraries
* [hyperlane-exex](https://github.com/aroralanuk/hyperlane-exex) ⭐ 14 | 🐛 0 | 🌐 Rust | 📅 2025-02-09, a PoC [Hyperlane](https://www.hyperlane.xyz) validator built as an ExEx ([Tweet](https://x.com/aroralanuk/status/1787203558955233562))
* [reth-exex-walltime](https://github.com/transmissions11/reth-exex-walltime) ⭐ 12 | 🐛 0 | 🌐 Rust | 📅 2024-08-05, an ExEx that provides compares block time (proposer clock) with wall time (local clock)
* [wvm-reth](https://github.com/weaveVM/wvm-reth) ⭐ 11 | 🐛 0 | 🌐 Rust | 📅 2025-06-13, a BigQuery ExEx ([blog post](https://docs.wvm.dev/about-weavevm/weavevm-testnet-v0))
* [exex-templates](https://github.com/weaveVM/exex-templates) ⭐ 10 | 🐛 0 | 🌐 Rust | 📅 2025-06-02, ExExes from the Load Network team
* [exex-nursery](https://github.com/jmcph4/exex-nursery) ⭐ 2 | 🐛 0 | 🌐 Rust | 📅 2025-03-20, a collection of ExExes that do interesting things
* [exex.rs](https://www.exex.rs), an open-source directory of ExExes ([blog post](https://blog.load.network/exex-rs-announcement/))

## Crawlers

A crawler (in the Ethereum context) is a program that indexes and gathers various metrics on different nodes within a P2P network (either at the execution or consensus layer).

* [reconnaissance](https://github.com/Will-Smith11/reconnaissance) ⭐ 92 | 🐛 0 | 🌐 Rust | 📅 2023-08-12, a proxy EL node using Reth
* [reth-crawler](https://github.com/Keep-Reth-Strange/reth-crawler) ⭐ 67 | 🐛 6 | 🌐 Rust | 📅 2024-02-03, a crawler for EL nodes ([Tweet](https://x.com/alemaz98/status/1731961719583396119))

## Indexers

An indexer (in the Ethereum context) takes data directly from the blockchain and produces alternative database schemas (typically relational) to allow enhanced and performant querying.

* [reth-indexer](https://github.com/joshstevens19/reth-indexer) ⭐ 506 | 🐛 15 | 🌐 Rust | 📅 2024-01-11, an indexer that accesses Reth's database directly and indexes into various backends

## Research

Publications using or mentioning Reth.

* [Decentralization of Ethereum’s Builder Market](https://arxiv.org/pdf/2405.01329), a paper due to Yang, et. al. that details the auction dynamics of [MEV-Boost](https://github.com/flashbots/mev-boost) ⭐ 1,439 | 🐛 86 | 🌐 Go | 📅 2026-06-30 auctions and the subsequent structure current PBS pipeline ([Tweet 1](https://x.com/gakonst/status/1787802487753154862), [Tweet 2](https://x.com/kartik1507/status/1791485547589857753))

* [Diving into the Reth p2p stack](https://research.chainbound.io/diving-into-the-reth-p2p-stack), a blog post by [Chainbound](https://chainbound.io) that details the Reth P2P stack.

## Layer 2

* [pevm](https://github.com/risechain/pevm) ⭐ 357 | 🐛 73 | 🌐 Rust | 📅 2026-08-05, a massively-parallelised EVM implementation by [RISE Labs](https://www.riselabs.xyz) that is explicitly compatible with Reth ([blog post](https://medium.com/@rise_chain/rise-pevm-parallel-evm-bdfc4bc9f38e), [Tweet](https://x.com/gakonst/status/1798165192460976195))
* [seismic-reth](https://github.com/SeismicSystems/seismic-reth) ⭐ 143 | 🐛 55 | 🌐 Rust | 📅 2026-09-03, node software for [Seismic](https://www.seismic.systems), the encrypted blockchain
* [Kakarot zkEVM](https://github.com/kkrt-labs/kakarot-rpc) ⚠️ Archived, a zkEVM built in Cairo (provable by design) for which the RPC component is constructed using Reth
* [grevm](https://github.com/Galxe/grevm) ⭐ 38 | 🐛 8 | 🌐 Rust | 📅 2026-08-18, parallel EVM runtime based on BlockSTM
* [rem-poc](https://github.com/adizere/rem-poc) ⭐ 20 | 🐛 0 | 🌐 Rust | 📅 2025-01-05, an integration with the [Malachite](https://github.com/informalsystems/malachite) ⭐ 10 | 🐛 12 | 🌐 Rust | 📅 2025-11-26 BFT consensus engine
* [reva](https://github.com/lita-xyz/reva) ⭐ 13 | 🐛 3 | 🌐 Rust | 📅 2025-07-02, minimal ZKP execution in Reth
* [sova-reth](https://github.com/SovaNetwork/sova-reth) ⭐ 1 | 🐛 1 | 🌐 Rust | 📅 2025-11-04, Reth but for Bitcoin
* [sp1-reth](https://github.com/succinctlabs/sp1-reth), a zkEVM PoC by [Succint Labs](https://succinct.xyz) demonstrating transaction costs to the order of $0.01 USD atop Reth
* [scroll-reth](https://x.com/gakonst/status/1788548434393210938), a port of Scroll to Reth

## Tutorials

* [reth-custom-api-example](https://github.com/libevm/reth-custom-api-example) ⭐ 29 | 🐛 1 | 🌐 Rust | 📅 2023-11-14, an example demonstrating RPC extension using Reth due to [libevm](https://libevm.com) ([blog post](https://www.libevm.com/2023/09/01/reth-custom-api))
  * This also became a talk during the hackathon at [ETHGlobal Sydney 2024](https://ethglobal.com/events/sydney)

## Presentations

* [RETH ExExs](https://docs.google.com/presentation/d/10VpdnTNKbhtip22UIAGNKchpPSi1E7ykI6Fb91d7jfg), presentation by [Roman Krasiuk](https://x.com/r_krasiuk) and [Yash Atreya](https://x.com/YashAtreya) at [EthCC 2024](https://x.com/wehack247), [Tweet 1](https://x.com/gakonst/status/1811443416674501061) [Tweet 2](https://x.com/YashAtreya/status/1811400954408833363)

### Devcon 2024

* [Reth 1.0: How did we get here and what is next?](https://www.youtube.com/watch?v=10xaWE28WCM), presentation by [Georgios Konstantopoulos](https://x.com/gakonst)
* [Using Reth Execution Extensions for next generation indexing](https://www.youtube.com/watch?v=GhEhzE9SFqY), presentation by [Alexey Shekhirin](https://x.com/ashekhirin)

## Miscellaneous

* [reth-payload-validator](https://github.com/ultrasoundmoney/reth-payload-validator) ⭐ 43 | 🐛 8 | 🌐 Rust | 📅 2024-12-13, a RPC extension of Reth by the [Ultra Sound Money relay](https://ultrasound.money) that implements rapid block validation of builder submissions
* [openvm-reth-benchmark](https://github.com/axiom-crypto/openvm-reth-benchmark) ⭐ 17 | 🐛 12 | 🌐 Rust | 📅 2026-09-03, a set of benchmarks for Reth within the OpenVM framework

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-09-03._
