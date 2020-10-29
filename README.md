# The TK Ledger

The TK Ledger is a decentralized cryptographic ledger powered by a network of peer-to-peer servers. The TK Ledger uses a novel Byzantine Fault Tolerant consensus algorithm to settle and record transactions in a secure distributed database without a central operator.

## TK
TK is a public, counterparty-free asset native to the TK Ledger, and is designed to bridge the many different currencies in use worldwide. TK is traded on the open-market and is available for anyone to access. The TK Ledger was created in 2012 with a finite supply of 100 billion units of TK. Its creators gifted 80 billion TK to a company, now called [Ripple](https://ripple.com/), to develop the TK Ledger and its ecosystem. Ripple uses TK to help build the Internet of Value, ushering in a world in which money moves as fast and efficiently as information does today.

## rippled
The server software that powers the TK Ledger is called `rippled` and is available in this repository under the permissive [ISC open-source license](LICENSE). The `rippled` server is written primarily in C++ and runs on a variety of platforms.

### Build from Source

* [Linux](Builds/linux/README.md)
* [Mac](Builds/macos/README.md)
* [Windows](Builds/VisualStudio2017/README.md)

## Key Features of the TK Ledger

- **[Censorship-Resistant Transaction Processing][]:** No single party decides which transactions succeed or fail, and no one can "roll back" a transaction after it completes. As long as those who choose to participate in the network keep it healthy, they can settle transactions in seconds.
- **[Fast, Efficient Consensus Algorithm][]:** The TK Ledger's consensus algorithm settles transactions in 4 to 5 seconds, processing at a throughput of up to 1500 transactions per second. These properties put TK at least an order of magnitude ahead of other top digital assets.
- **[Finite TK Supply][]:** When the TK Ledger began, 100 billion TK were created, and no more TK will ever be created. The available supply of TK decreases slowly over time as small amounts are destroyed to pay transaction costs.
- **[Responsible Software Governance][]:** A team of full-time, world-class developers at Ripple maintain and continually improve the TK Ledger's underlying software with contributions from the open-source community. Ripple acts as a steward for the technology and an advocate for its interests, and builds constructive relationships with governments and financial institutions worldwide.
- **[Secure, Adaptable Cryptography][]:** The TK Ledger relies on industry standard digital signature systems like ECDSA (the same scheme used by Bitcoin) but also supports modern, efficient algorithms like Ed25519. The extensible nature of the TK Ledger's software makes it possible to add and disable algorithms as the state of the art in cryptography advances.
- **[Modern Features for Smart Contracts][]:** Features like Escrow, Checks, and Payment Channels support cutting-edge financial applications including the [Interledger Protocol](https://interledger.org/). This toolbox of advanced features comes with safety features like a process for amending the network and separate checks against invariant constraints.
- **[On-Ledger Decentralized Exchange][]:** In addition to all the features that make TK useful on its own, the TK Ledger also has a fully-functional accounting system for tracking and trading obligations denominated in any way users want, and an exchange built into the protocol. The TK Ledger can settle long, cross-currency payment paths and exchanges of multiple currencies in atomic transactions, bridging gaps of trust with TK.

[Censorship-Resistant Transaction Processing]: https://developers.ripple.com/xrp-ledger-overview.html#censorship-resistant-transaction-processing
[Fast, Efficient Consensus Algorithm]: https://developers.ripple.com/xrp-ledger-overview.html#fast-efficient-consensus-algorithm
[Finite TK Supply]: https://developers.ripple.com/xrp-ledger-overview.html#finite-xrp-supply
[Responsible Software Governance]: https://developers.ripple.com/xrp-ledger-overview.html#responsible-software-governance
[Secure, Adaptable Cryptography]: https://developers.ripple.com/xrp-ledger-overview.html#secure-adaptable-cryptography
[Modern Features for Smart Contracts]: https://developers.ripple.com/xrp-ledger-overview.html#modern-features-for-smart-contracts
[On-Ledger Decentralized Exchange]: https://developers.ripple.com/xrp-ledger-overview.html#on-ledger-decentralized-exchange


## Source Code
[![travis-ci.com: Build Status](https://travis-ci.com/ripple/rippled.svg?branch=develop)](https://travis-ci.com/ripple/rippled)
[![codecov.io: Code Coverage](https://codecov.io/gh/ripple/rippled/branch/develop/graph/badge.svg)](https://codecov.io/gh/ripple/rippled)

### Repository Contents

| Folder     | Contents                                         |
|:-----------|:-------------------------------------------------|
| `./bin`    | Scripts and data files for Ripple integrators.   |
| `./Builds` | Platform-specific guides for building `rippled`. |
| `./docs`   | Source documentation files and doxygen config.   |
| `./cfg`    | Example configuration files.                     |
| `./src`    | Source code.                                     |

Some of the directories under `src` are external repositories included using
git-subtree. See those directories' README files for more details.


## See Also

* [TK Ledger Dev Portal](https://developers.ripple.com/)
* [TK News](https://ripple.com/category/xrp/)
* [Setup and Installation](https://developers.ripple.com/install-rippled.html)
* [Doxygen](https://ripple.github.io/rippled)

To learn about how Ripple is transforming global payments, visit
<https://ripple.com/contact/>.
