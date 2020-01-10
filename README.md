![Hyperledger Aries](collateral/Hyperledger_Aries_Logo_Color.png)

Hyperledger Aries allows trusted online peer-to-peer interactions based on
decentralized identities and verifiable credentials. Aries includes a protocol
definition, tools, and reference implementations. The Aries protocol supports
identities rooted in a variety of distributed ledgers or blockchains. This
approach to identity is often called Self Soverign Identity (SSI).

Key components of an Aries solution are:
* [agents](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0004-agents/README.md),
* [DID communications](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0005-didcomm/README.md),
* [protocols](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0003-protocols/README.md) 
* and [key management](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0051-dkms/README.md)

# Getting Started

Aries is a young project that is maturing quickly. Documentation and links are
often out-of-date.

The most consistently maintained guide for new developers is the one included in
the Aries Cloud Agent Python (ACApy):

https://github.com/hyperledger/aries-cloudagent-python/tree/master/docs/GettingStartedAriesDev

There is also an EdX course here:

https://www.edx.org/course/identity-in-hyperledger-aries-indy-and-ursa

# Repos

The Aries project contains a number of repos, which can be grouped into some
important categories.

## Agents

Most developers who want to solve business problems should start with an agent.
The Aries project provides some open source agents, but there are other Aries
compatible agents available through their developers.

* [aries-cloudagent-python](https://github.com/hyperledger/aries-cloudagent-python/blob/master/README.md)
* [aries-staticagent-python](https://github.com/hyperledger/aries-staticagent-python)

## Language Frameworks

If none of the off-the-shelf agents work for your use case, you should look at
developing your own agent using one of the language frameworks.

* [aries-framework-dotnet](https://github.com/hyperledger/aries-framework-dotnet/blob/master/README.md)
* [aries-framework-go](https://github.com/hyperledger/aries-framework-go/blob/master/README.md)
* [aries-sdk-ruby](https://github.com/hyperledger/aries-sdk-ruby/blob/master/README.md)
* [aries-framework-javascript](https://github.com/hyperledger/aries-framework-javascript/blob/master/README.md)

## Development Tools and Test Suites

The Aries project provides some useful tools for developing agents and testing
that they are compatible with other agents in the ecosystem.

* [aries-toolbox](https://github.com/hyperledger/aries-toolbox)
* [aries-protocol-test-suite](https://github.com/hyperledger/aries-protocol-test-suite)

## Shared Libraries

*Coming Soon*
There are also a set of shared open source libraries that provide C-callable
APIs that can be used by agents and frameworks to support the Aries protocols.

* Aries Key Management: Functions for managing keys, including storage plugins.
* Aries Verifiable Data Registry Interface: An interface for verifying data
  agianst an underlying ledger.
* Aries Util: Utility functions for Aries communication, such as message
  packing.

## Protocols

If you want to understand the theory and the [open standards that these agents
and frameworks
implement](https://github.com/hyperledger/aries-rfcs/blob/master/index.md), then
you should refer to the Aries protocol documents:

* [aries-rfcs](https://github.com/hyperledger/aries-rfcs)

# Project Participation

You can raise issues using the GitHub issue tracker in each Aries repository.
Pull requests are appreciated; please review CONTRIBUTING.md for the repository
to which you want to contribute.

You can reach other Aries developers:
* in the RocketChat channel
  [#aries](https://chat.hyperledger.org/channel/aries),
* on the [mailing list](https://lists.hyperledger.org/g/aries),
* or in the [Aries Working Group](https://wiki.hyperledger.org/display/ARIES/Aries+Working+Group) weekly call.

# Relationship to Hyperledger Indy

Aries grew out of the work in [Hyperledger
Indy](https://github.com/hyperledger/indy-sdk/blob/master/README.md) to create
technologies for managing decentralized identity. Indy provides a [specific
blockchain purpose-built for
identity](https://github.com/hyperledger/indy-node/blob/master/README.md). The
tools created in Indy for building agents are being migrated to Aries, and
extended to be blockchain-agnostic. Functionality related to the Indy ledger
will remain in Indy.

If you are already using Indy SDK to build a decentralized identity solution,
you can keep using it knowing that it will continue to be maintained while the
Aries tools mature. When the Indy SDK is deprecated, a reasonable transition
process will be communicated.
