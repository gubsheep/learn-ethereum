---
title: "[Tutorial] Setting up your first wallet"
date: 2018-10-29T10:15:01+02:00
language: en
slug: setting-up-wallet
weight: 3
---

# Setting up your first wallet

I’ve found working with MetaMask to be a user-friendly and secure way to manage my Ethereum accounts. 

## Install MetaMask

Go to the [Chrome Web Store](https://chrome.google.com/webstore/search/metamask) and install the MetaMask extension.

From time to time there are other extensions named “MetaMask” that are branded similarly, which are likely to be phishing scams. You’re fine if you install the MetaMask extension that clearly has the appropriate number of downloads and ratings. 

## Create an Account

After installation, follow the instructions to set up your first account. A few things that I think are important to note:

- Your MetaMask password is a password for accessing the extension’s *local* storage data. You can’t go onto someone else’s computer, open up MetaMask, enter your password, and gain access to your Ethereum account. This password is more analogous to the password you’d use to log in to your computer, rather than the password you’d use to log into Facebook from any device.
- If you delete the MetaMask extension, the extension’s local storage is deleted - this includes your public and private keys!! 
- However, upon account creation, MetaMask generates a “seed phrase” for you which can be used to restore your private key from a MetaMask extension on any device. The MetaMask extension implements a one-to-one function to derive private keys from seed phrases, so as long as you write your seed phrase down and keep it somewhere safe, you’ll always have access to your private key if you can get your hands on a device with MetaMask.