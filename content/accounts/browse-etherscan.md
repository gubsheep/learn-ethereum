---
title: "[Tutorial] Browse account data with Etherscan"
date: 2018-10-29T10:15:01+02:00
language: en
slug: browse-etherscan
weight: 4
---

# Browse Account Data with Etherscan

Etherscan is a helpful web application that allows you to view information about the blockchain in a human-readable way.

The entire history of all transactions, blocks, accounts, code, and other metadata collectively make up the “blockchain,” which is stored on every single Ethereum node. Etherscan.io runs a few nodes of their own, and thus has a copy of the entire blockchain on its machines. Etherscan then surfaces all of this data in a webapp.

We can use Etherscan to find information about different accounts:

- Your own account: Open MetaMask, click the three dots next to your account name (by default the account name is “Account 1”), and click “View account on Etherscan.” This opens up a URL that looks something like: https://etherscan.io/address/[ADDRESS]. In this way you can view the transaction history and balance of your own account (which is also available in MetaMask). Replacing the address in the URL allows you to see the data associated with *any* account. If you’ve just created your account, Etherscan should show a balance of 0 ETH and no previous transactions.
- [An account I own](https://etherscan.io/address/0x85d918c2b7f172d033d190152aec58709fb6d048): This is an account with address 0x85d918c2B7F172d033D190152AEc58709Fb6D048. In the past I’ve used it to send Ether to people who have read and given feedback on my articles! You can see that it has a nonzero balance.

*more on precisely what it means to be a “node” later - for now, think of nodes as the computers that are storing the blockchain, broadcasting transaction requests, executing others’ transactions and code, and synchronizing with each other on the Ethereum network