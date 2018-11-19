---
title: The Current State of Ethereum
date: 2018-10-29T10:15:01+02:00
language: en
slug: current-state
weight: 3
---

# The current state of Ethereum
As of late November 2018, Ethereum is largely still in a proof-of-concept state.

## Are there apps built to run on Ethereum that are presently providing significant value to end users?

The short answer is no. Most DApps presently are prototypes or proofs-of-concept and aren’t yet competitive with their centralized counterparts. You can check out a curated list of DApps [here](https://www.stateofthedapps.com/). [CryptoKitties](https://www.cryptokitties.co/) and [Augur](https://www.augur.net/) are examples of DApps.

Ethereum development is in the very, *very* early stages. This contrasts with Bitcoin, which is already providing a lot of its intended value-add to the world and whose base level protocol has (some claim) more-or-less matured. The intended value-add of Ethereum to the world is still very far off. My personal prediction is that the first “real” DApps are at least 2 years off.

## Who actually executes the code of a DApp?

Every node on the network executes all the backend code of every DApp. So, if your machine is running a full node, it’s running the backend of 1,500+ DApps simultaneously. 30,000+ other full nodes are also running the exact same 1,500+ DApp backends.  

## What is the current performance of the EVM?

At present, the Ethereum network (and by extension, the EVM) can’t execute more than about 10 transactions per second. Concretely, a “transaction” is a write to permanent storage on the blockchain; for example, any transfer of Ether or other tokens between accounts is a transaction. The execution speed of the EVM is firstly upper-bounded by the speed of the miners/full nodes; in practice it is in fact much much lower, because of the proof-of-work required. This makes Ethereum in present form unusable for most large-scale applications.

## How does Ethereum plan to handle larger-scale services?

The Ethereum core researchers/developers are working on performance solutions including Plasma, Sharding, and Proof-of-Stake consensus protocols which may (potentially) improve performance by 4 or more orders of magnitude. 

## What is Ethereum’s relationship with “ICO”s and “altcoin”s?

Many altcoins and most ICOs are actually built on the Ethereum network. Because Ethereum allows for the creation and execution of arbitrary programs, creating a token for an ICO is as simple as deploying a program to the Ethereum network that keeps track of who owns how much of the token in persistent EVM storage. Notably, this is much easier to do on top of Ethereum than on top of Bitcoin.

