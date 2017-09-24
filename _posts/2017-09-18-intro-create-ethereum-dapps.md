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

![testrpc_run]({{ site.url }}/assets/img/1_testrpc_run.PNG)

We want to keep this powershell window open.

So now that we have our test accounts up and running, each with 100 ether let's try to get some info about these accounts by using the Ethereum's JavaScript API - web3. Open up new powershell window, run `node` then the following commands:

{% highlight powershell %}
var Web3 = require('web3');
var web3 = new Web3('http://localhost:8545');
web3.eth.getAccounts().then(console.log);
{% endhighlight %}

This should return an array of ethereum addresses that testrpc is serving up to us. These are 40 hex characters that correspond to an individual's public key.

![web3_getAccounts]({{site.url}}/assets/img/2_web3_getAccounts.PNG)





