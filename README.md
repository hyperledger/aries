![Hyperledger Aries](collateral/Hyperledger_Aries_Logo_Color.png)

#### Migration Notice
>Aries Code Repositories are in the process of being migrated from various other locations, including Hyperledger Indy repositories where the Aries work was incubated. Some of the code requires refactoring work to split it from unrelated assets prior to migration.

>The status of these code migrations is under regular discussion on the [#aries](https://chat.hyperledger.org/channel/aries) and [#indy-agent](https://chat.hyperledger.org/channel/indy-agent) channels on chat.hyperledger.org and in the [Aries Working Group](https://wiki.hyperledger.org/display/ARIES/Aries+Working+Group) weekly call. Please join us there to understand migration status and help identify places where help is needed.

>When the appropriate code is migrated to this repoisitory, this README file will be updated.

#
Hyperledger Aries is a blockchain-agnostic, reference implementation of the
[agent](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0004-agents/README.md)
[DID communications](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0005-didcomm/README.md),
[wallet](
),
[protocols](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0003-protocols/README.md) 
and
[key management](
https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0051-dkms/README.md)
technologies that underpin decentralized identity.

### Repos

Aries work is spread across many repos. Most developers who want to solve business
problems with decentralized identity should start with an agent framework such as:

[TODO: THESE LINKS ARE NOT YET ACTIVE]

* [aries-agent-python](https://github.com/hyperledger/aries-agent-python)
* [aries-agent-java](https://github.com/hyperledger/aries-agent-java)
* [aries-agent-nodejs](https://github.com/hyperledger/aries-agent-nodejs)
* [aries-agent-dotnet](https://github.com/hyperledger/aries-agent-dotnet)
* [aries-agent-rust](https://github.com/hyperledger/aries-agent-rust)

If you want to understand the theory and the open standards that these frameworks
implement, then you should visit:

* [aries-rfcs](https://github.com/hyperledger/aries-rfcs)

If you want to work on the low-level features that underpin all the agent
frameworks, then the repo you want is:

* [aries-sdk](https://github.com/hyperledger/aries-rfcs)

### Relationship to Hyperledger Indy

Hyperledger Indy is all about decentralized identity, like Aries. However, Indy is
focused on a specific blockchain purpose-built for identity, whereas Aries is
blockchain-agnostic.

Much of the work done in Indy SDK between 2017 and 2019 was actually blockchain-agnostic,
and the developers in that community began formalizing many concepts related to agents
and DIDComm. Now that Aries exists, Indy artifacts will be partitioned. Functionality
related to Indy's blockchain will remain in Indy, whereas general functionality will be
moved over to Aries repos through a PR process for broader community ratification.

If you are using Indy SDK today to build a decentralized identity solution, keep
doing so for the time being. Aries is not yet mature enough to build upon, but when
it gets there, a reasonable transition process will be provided, and announcements will
be made in community channels.

