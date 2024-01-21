# The tiny garden protocol (TGP) [WIP]
**This document is beyond done, it will be subject to heavy change. PRs and ideas are welcome**

TGP should provide a reliable, encrypted, decentralized, asynchronous, multi-device messaging system.
However, unlike common chat protocols of this fashion, it is a non-goal to provide a system of untrusted home-servers interacting with another.
Instead, TGPs goal is to provide the means of creating limited, controlled and trusted messaging networks, in which users are able to freely interact within. It is an explicit non-goal (at this point in time) to provide inter-network messaging.

The idea of TGP is to provide private messaging to communities and companies on the web and on site networks.

## Goals
### Messaging
As TGP is about text-based communication, the limits of TGP target scope should be well-defined.

The primary goal, as of every text-based communication protocol, is in the end, the sending and receiving of messages between two or more parties, limitations and requirements of this are to be elaborated on in this section.

Additionally, as modern protocols have evolved beyond the needs of simple text transfer, the protocol may support file transfers and should be open for future expansions such as voice or video communication, e.G. via a TURN integration. 

### Reliability & decentralization
TGP tries to achieve reliability through the means of decentralization.
Specifically, networks are formed of at minimum one server, also known as a **node**.
Nodes in TGP are for the most parts transparent to the Client, as the client only has to decide to which node of a network it wants to connect.

#### Requirements and limitations
- Nodes trust each other, this trust must be established cryptographically
- Nodes must be able to communicate securely over the internet as they may be spread beyond the limits of a local network
- Multiple nodes belonging to the same network should not run on the device

### Cryptography
MLS (message layer security) will be used in all of TGP.

### Asynchronicity & multi-device
- Allow for messaging offline users
- Messages history must be preserved
- Users may use multiple devices for the same account

### Networks

## Specification
### Inter-node communication
- Noise protocol
- Nodes have set keys they use for noise which they also use as proof of identity
