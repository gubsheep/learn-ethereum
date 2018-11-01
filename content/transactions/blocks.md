---
title: "Transactions are committed to the network in batches, or “blocks”"
date: 2018-10-29T10:15:01+02:00
language: en
slug: blocks
weight: 3
---

# Transactions are committed to the network in batches, or “blocks”

Dozens of transaction requests are propagated around the Ethereum network per second. Simultaneously, miners verify, execute, and propagate state change associated with dozens of transactions per second. Because of latency and the nature of the network, it may be the case that two miners hear about, execute, and start propagating the result of two different local transactions before they hear about each others’. Given this, how do we ensure that all participants on the network maintain a synchronized state and agree on the precise history of transactions?

One solution is by batching transactions, so that batches of dozens (or hundreds) of transactions are committed, agreed on, and synchronized on all at once. By spacing out commits, we give all network participants enough time to come to consensus—though transaction requests occur dozens of times per second, batches on Ethereum are committed approximately once every fifteen seconds. We call these batches *blocks*. To preserve the transaction history, blocks are strictly ordered (every new block created contains a reference to its parent block), and transactions within blocks are strictly ordered as well. Except in rare cases, at any given time, all participants on the network are in agreement on the exact number and history of blocks, and are working to batch the current live transaction requests into the next block. 

Once a block is put together (*mined*) by some miner on the network, it is propagated to the rest of the network; all nodes add this block to the end of their *blockchain*, and mining continues. The exact block-assembly (mining) process is specified in by the “Proof-of-Work” protocol, whose details ensures that blocks are almost always proposed one at a time by miners. Proof-of-Work also provides additional security guarantees and cryptoeconomic incentives, though we won’t cover those in this section.

As a second incentive for miners to contribute their computational resources to the network, the Ethereum specification awards a “free” transaction of 3 Ether to whoever mines the next block. The miner of a block can include a 3 Ether transaction to themselves, essentially out of thin air.