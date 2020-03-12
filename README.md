![Hyperledger Aries](collateral/Hyperledger_Aries_Logo_Color.png)

Hyperledger Aries allows trusted online peer-to-peer interactions based on
decentralized identities and verifiable credentials. Aries includes a protocol
definition, tools, and reference implementations. The Aries protocol supports
identities rooted in a variety of distributed ledgers or blockchains. This
approach to identity is often called Self Sovereign Identity (SSI).

Key components of an Aries solution are:
* [agents](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0004-agents/README.md),
* [DID communications](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0005-didcomm/README.md),
* [protocols](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0003-protocols/README.md) 
* and [key management](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0051-dkms/README.md)

## Getting Started

Aries is a young project that is maturing quickly. As such, be warned that the
project documentation and links may get out of out-of-date. If you find there is
something missing, please connect with the community on the [Aries Hyperledger
Rocketchat Channel](https://chat.hyperledger.org/channel/aries). And of course,
pull requests are always welcome to fix things that are confusing!

If you are entirely new to the decentralized identity space and the Hyperledger
projects there is a [Linux Foundation edX course on decentralized identity and
Hyperledger Indy, Aries and
Ursa](https://www.edx.org/course/identity-in-hyperledger-aries-indy-and-ursa).
Start there! A companion developers edX course is planned for "early" 2020.

If you know about decentralized identity and verifiable credentials and want to
get started building applications on top of Aries (and Indy), the most
consistently maintained [guide for new
developers](https://github.com/hyperledger/aries-cloudagent-python/tree/master/docs/GettingStartedAriesDev)
is the one included in the Aries Cloud Agent Python (ACApy):

## Repos

The Aries project contains a number of repos, which can be grouped into some
important categories.

### Aries Agent Frameworks

Developers who want to solve business problems (vs. contributing directly to Aries) should start with an Aries agent framework. Agent-based applications are created by adding application-specific code that control the Aries agent.

There are several Aries general purpose agent frameworks that are ready to go out of the box.

- [Aries Cloud Agent -
  Python](https://github.com/hyperledger/aries-cloudagent-python) (ACA-Py) is
  suitable for all non-mobile agent applications and has production deployments.
  ACA-Py and a controller run together, communicating across an HTTP interface.
  Your controller can be written in any language and ACA-Py embeds the Indy-SDK.
- [Aries Framework -
  .NET](https://github.com/hyperledger/aries-framework-dotnet) can be used for
  building mobile (via [Xamarin](https://dotnet.microsoft.com/apps/xamarin)) and
  server-side agents and has production deployments. The controller for an
  aries-framework-dotnet app can be written in any language supporting embedding
  the framework as a library in the controller. The framework embeds the
  Indy-SDK.
- [Aries Static Agent -
  Python](https://github.com/hyperledger/aries-staticagent-python) is a
  configurable agent that does not use persistent storage.

There are several other frameworks that are currently under active development, including:

- [Aries Framework - Go](https://github.com/hyperledger/aries-framework-go) is a
  pure golang framework that provides a similar architecture to ACA-Py, exposing
  an HTTP interface for it's companion controller. The framework does not
  currently embed the Indy SDK and work on supporting a golnag-based verifiable credentials implementation is in progress.
- [aries-sdk-ruby](https://github.com/hyperledger/aries-sdk-ruby/blob/master/README.md)
- [aries-framework-javascript](https://github.com/hyperledger/aries-framework-javascript/blob/master/README.md)

### Development Tools and Test Suites

The Aries project provides some useful tools for developing agents and testing
that they are compatible with other agents in the ecosystem.

* [aries-toolbox](https://github.com/hyperledger/aries-toolbox)
* [aries-protocol-test-suite](https://github.com/hyperledger/aries-protocol-test-suite)

### Shared Libraries

*Coming Soon*
There are also a set of shared open source libraries that provide C-callable
APIs that can be used by agents and frameworks to support the Aries protocols.

* Aries Key Management: Functions for managing keys, including storage plugins.
* Aries Verifiable Data Registry Interface: An interface for verifying data
  agianst an underlying ledger.
* Aries Util: Utility functions for Aries communication, such as message
  packing.

While these are in development, the ACA-Py and .NET frameworks embed the Indy-SDK, while the Go framework is building the capabilities in golang.

### Protocols

If you want to understand the theory and the [open standards that these agents
and frameworks
implement](https://github.com/hyperledger/aries-rfcs/blob/master/index.md), then
you should refer to the Aries protocol documents:

* [aries-rfcs](https://github.com/hyperledger/aries-rfcs)

## Project Participation

You can raise issues using the GitHub issue tracker in each Aries repository.
Pull requests are appreciated; please review CONTRIBUTING.md for the repository
to which you want to contribute.

You can reach other Aries developers:
* in the RocketChat channel
  [#aries](https://chat.hyperledger.org/channel/aries),
* on the [mailing list](https://lists.hyperledger.org/g/aries),
* or in the [Aries Working Group](https://wiki.hyperledger.org/display/ARIES/Aries+Working+Group) weekly call.

## Relationship to Hyperledger Indy

Aries grew out of the work in [Hyperledger
Indy](https://github.com/hyperledger/indy-sdk/blob/master/README.md) to create
technologies for managing decentralized identity. Indy provides a [specific
blockchain purpose-built for
identity](https://github.com/hyperledger/indy-node/blob/master/README.md). The
tools created in Indy for building agents are being migrated to Aries, and
extended to be blockchain-agnostic. Functionality related to the Indy ledger
will remain in Indy.

If you want to start build decentralized identity capabilities around Indy, you
should use the existing Aries Agent frameworks described above that embed the
Indy SDK. If you are already using the Indy SDK to build a decentralized
identity solution, you can keep using it knowing that it will continue to be
maintained. If and when the Indy SDK is fully or partially deprecated, a
transition process will be communicated.
