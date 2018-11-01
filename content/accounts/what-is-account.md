---
title: What is an account?
date: 2018-10-29T10:15:01+02:00
language: en
slug: what-is-account
weight: 1
---

# What is an account?

In Ethereum, an *account* is an object which holds ether and possibly other metadata. It is slightly more general than the traditional concept of a financial “account” (i.e. an account on a bank or payment service). At a basic level, an account contains:

- An **address**: a 20-byte unique identifier. Anyone on the network can look up an account and its associated balance/metadata using this identifier. 
- A **balance**: the amount of ether “owned” by this account.
- **Metadata**: the number of transactions this account has participated in, and other associated data or code. 

Ethereum supports two different types of accounts: user-owned accounts (accounts managed by users), and smart contract accounts (accounts with programmed-in behavior). 

- User-owned accounts (or “externally-owned accounts”) are exactly what they sound like, and map closely to the traditional notion of a payment system account. A human or human entity owns the account and uses it to hold ether and initiate transactions. Note that one person can distribute their funds over multiple user-owned accounts (this is in fact good practice if you own a lot of ether). The keys required to access a user-owned account are stored in a *wallet*, which will be discussed later. 
- “Contract accounts” are assigned by the Ethereum network to any smart contract deployed to the network. These accounts wrap the smart contract code, and hold any persistent data associated with the smart contract program. At a high level, execution of this code can be automatically triggered by any user by sending ether and input data from their user-owned accounts to the contract account.

Earlier we mentioned that Ethereum is a computer (the EVM), and that the Ethereum computer’s storage contains a record of all transactions/code that the computer has executed as well as the current state of the computer. The state of the computer at any time includes the data of every account that exists on the Ethereum network at that time, indexed by their addresses. Therefore, anyone who stores the state of the EVM locally can look up the data (such as the balance) associated with any account address.

An account is *not* a wallet. A wallet is the keypair associated with a user-owned account, which allow a user to make transactions from or manage the account. Wallets will be discussed shortly.
