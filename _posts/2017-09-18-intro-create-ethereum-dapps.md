---
layout: post
title: 'Create your own cryptocurrency using Ethereum DApps'
subtitle: 'Intro about how to create a simple cryptocurrency using Ethereum DApps'
date: 2017-09-17
categories: ethereum
cover: 'https://media.coindesk.com/uploads/2016/02/Screen-Shot-2016-02-24-at-10.42.13-AM-e1456328600212.png'
tags: ethereum cryptocurrency blockchain
---

### Welcome

To start from scratch without using any DApp frameworks we'll need to install a few things to get us up and running with testrpc. Testrpc  creates a local instance of the ethereum blockchain with accounts for testing; it allows you to deploy and test your contract without interacting with the real chain (which we will get to in part 2).

I'm currently running this on a fresh Windows 10 machine. I followed Prateesh's steps for installing testrpc on Windows 10: [steps-to-install-testrpc-in-windows-10](https://medium.com/@PrateeshNanada/steps-to-install-testrpc-in-windows-10-96989a6cd594)

Once ethereumjs-testrpc and web3 modules are installed we can spin up the testrpc chain: 

![testrpc_run]({{ site.url }}/assets/img/1_testrpc_run.png)
