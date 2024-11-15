# nostr-algorithms-research
A collection of research studies into algorithms for Nostr, including Web of Trust, and more.

## What is Nostr

[Nostr](https://github.com/nostr-protocol/nostr) is a simple but powerful new protocol for building social apps, that works by sending standardized and cryptographically signed JSON events to several servers called "relays".

This novel approach unlocks new opportunities and brings several benefits, including (but not limited to):
1. Since anyone can build on the protocol, the social media experience can customized to fit specific needs of individuals and businesses.
2. Users can choose the apps they use and the servers they connect to, and bring along their data and digital social identity with them, which cannot be done with centralized social media platforms.
3. App developers can create new social applications and reuse existing social graphs, overcoming network effect cold start problems that many new such apps face.
4. Users have more control and sovereignty over their own digital identity.
5. There is more opportunity to build healthier social applications. Most centralized social applications collect big amounts of private data from their users and use that to keep them engaged and sell them ads, mostly due from their ad-based revenue model — a practice that many people have begun to question. Nostr brings more opportunities to build healthier apps and revenue models that don't lead to these same detrimental effects.

### Challenges

Being a new network, Nostr still faces certain challenges, including:
1. **Sybil attacks and impersonation:** Creating new identities is as easy as generating a cryptographic keypair. Since there is no central authority to verify users.
2. **Spam prevention:** Relay operators usually have measures to prevent spam, but since new identities are so easy to make, LLMs can be used to generate plausible content, and free relay operators usually have limited financial resources, this remains a challenge.
3. **Content moderation:** Given that users can choose any relays they wish, they may experience varying degrees of content moderation quality, which may depend on the resources available to the relay operators and willingness to moderate — and also due to the partly subjective nature of what people want and don't want to see.

In centralized networks, these issues are resolved by a central authority in the system (i.e. the company that runs it). For a decentralized network to remain decentralized, new approaches are needed.

### Web of Trust (WoT)

Web of Trust is a concept that attempts to address some of the above issues without introducing centralization, by having a web of people trusted by the user to collectively decide what to show/recommend, and what to hide/block. The analogy is that "If many friends recommends something, it is more likely a good thing. Conversely, if many friends recommend against something, it is better to block it".

It is currently one of the most promising algorithms to tackle these problems.

## What is this repository

This repository will hold some data-driven studies on algorithms that aim to help improve discoverability, usability, safety, controllability and spam detection, including WoT algorithms. The goal is to better understand the effects of these, and the dynamics of the network as a whole.

