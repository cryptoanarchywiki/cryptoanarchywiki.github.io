---
layout: static-informational
permalink: /getting-started/what-is-bitcoin
title: What is Bitcoin (And How is it Related)?
categories: [getting-started]
---

Wikipedia defines "[Bitcoin](https://en.wikipedia.org/wiki/Bitcoin)" as follows (2018-05-26):

> Bitcoin (₿) is a cryptocurrency and worldwide payment system. It is the first decentralized digital currency, as the system works without a central bank or single administrator. The system was designed to work as a peer-to-peer network, a network in which transactions take place between users directly, without an intermediary. These transactions are verified by network nodes through the use of cryptography and recorded in a public distributed ledger called a blockchain. Bitcoin was invented by an unknown person or group of people under the name Satoshi Nakamoto and released as open-source software in 2009.

During the 90s era of the Cypherpunks Mailing List, most of the components that cypherpunks felt were necessary were largely solved and fleshed out. These included chains anonymous remailers which allowed users to send email anonymously without recipient, or any of the remailers, being able to link sender, content and recipient. This technology was essentially a precursor to the "onion routing" used in the Tor anonymity network.

One, absolutely essential, tool still eluded them though: digital cash. Academic cryptographer David Chaum had made some progress towards a digital cash system that gave transactional privacy to participants, however there was one major problem with all the known systems at the time. They all had central points of failure which governments could shut down. [E-gold](https://en.wikipedia.org/wiki/E-gold), was essentially an anonymous digital cash system that was issued (and backed with physical gold) by a company of the same name. This ended with criminal prosecution of the company's founders by the US Government as unlicensed money transmitters.

Cypherpunks were left without this piece of their puzzle until 2008, when a person (or group) operating under the pseudonym "Satoshi Nakamoto" released a whitepaper detailing a viable solution to the problem. "[Bitcoin: A Peer to Peer Electronic Cash System](https://bitcoin.org/bitcoin.pdf)" outlined a system which was fully peer to peer (i.e. it had no central point of failure). Traditionally, a central authority had been required to ensure that the unit of e-cash was not "double-spent".

To better understand the problem. Consider that to spend your unit of e-cash, you simply cryptographically sign it over to someone else and transmit that information to them. The money would then exist as a verifiable chain of cryptographic signatures (the transactions) going back to the issuer of that unit of e-cash. However there is a huge problem with this approach:

+ What is to stop you from making a copy, and signing the same unit of e-cash over to two different people?
+ How would those two people discover discover the existence of the other's transaction? i.e. that the chain had forked, duplicating that unit of e-cash.

Bitcoin solved this problem via a global ledger that all network participants must agree upon. There are some very sophisticated game-theoretical incentives built into the system to keep everyone honest and using the same version of the ledger. I won't dive too much deeper into the details of how this works, but every ten minutes a new "block" of transactions is added to the ledger. If your transaction is included in that block, then the network will not accept an attempt to double-spend. This is because the network is now in agreement that you no longer own that unit of e-cash.

This was a revolutionary discovery that re-engergised the now largely stagnant cypherpunk movement. It is highly likely that Satoshi Nakamoto is someone (or someones) who was active on the Cypherpunks Mailing List during its 90s heyday, and spent the next 10-15 years in the search of a solution. At this point it seems very unlikely we'll ever know who was behind the "Satoshi Nakamoto" pseudonym, which is, in a way, a great shame since their story is one that would almost-certainly be fascinating to hear. However, being birthed by a pseudonymous creator couldn't be a more "cypherpunk" beginning to the project.

From Bitcoin, this paradigm shift has spawned innumerable immitations and attempted improvements on the underlying technology, many of which now have market-caps significantly exceeding $1 billion USD. Bitcoin itself has a market cap of over $128 billion USD at time of writing (2018-05-27).

With a solution to its intractable problem, this ignited a wave of new interest in the ideas associated with the cypherpunk movement. A new generation of people who were children or not-yet-born during the 90s are now exploring the possibilities opened up by uncensorable, pseudonymous digital cash and strong anonymity/privacy.

It is those people, technology historians, and nostalgic old-timers who are the intended readers of this site.

## tl;dr:

+ Essential reading: [Bitcoin: A Peer to Peer Electronic Cash System](https://bitcoin.org/bitcoin.pdf)
+ The cypherpunk movement stalled in its quest for social change due to a lack of good, uncensorable, anonymous (or at least pseudonymous) e-cash without a central point of failure that nation states could attack.
+ Traditionally, cryptographic e-cash systems have relied upon a central authority to detect and reject attempts to "double-spend" the same unit of e-cash.
+ Bitcoin solved this problem by finding a cryptographic and game-theoretical incentive structure which allows network participants to agree upon a ledger of e-cash ownership at any given time.
+ Now that the cypherpunks' central roadblock has been overcome, this has ignited a huge wave of new interest in their ideas.
