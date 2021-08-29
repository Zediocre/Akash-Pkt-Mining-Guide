
# Akash/Pkt Mining-Guide (in 5 Minutes)
Easy to use step by step guid to mine Pkt
Deploying a PKT miner (easily)

## Table of Contents
 - [Prerequisites](#prerequisites)
 - [Setting up the tool](#setting-up-the-tool)
 - [Deploying](#deploying)
 - [Deploying your own application](#deploying-your-own-application)
## Prerequisites
 - A PKT wallet. I use [this](http://pkt.world/wallet) one.
 - Some AKT tokens. I would recommend minimum 10.
 - Windows or MacOS
 
## Setting up the tool

 - Download and install [this](https://www.akashlytics.com/deploy) tool.
 - Go through the on-screen instructions as on how to create/restore a wallet.
 - Send over some AKT.
 - Create a certificate near the top right corner.

## Deploying

 - Copy the contents from [this](https://github.com/ovrclk/pkt-miner/blob/main/deploy.yaml) file.
 - In the tool, go to `Deployments` > `Create Deployment`.
 - Navigate forward by pressing Next > Empty <sub><sup>(An empty template with some basic config to get started.)</sub></sup> > Continue.
 - Paste the contents we copied in the first step.
 - Swap out the <PKT_WALLET> from `WALLET_ADDR=<PKT_Wallet>` to your wallet. It will look similar to this: `WALLET_ADDR=pkt1q76e5rqurp7lhpvqcnvvuwsuckqcrzsn9hlxdyc`.
 - Swap out the latest to v1.0.0 from `image: chandrastation/pkt_on_akash:latest`. It should look like this `image: chandrastation/pkt_on_akash:v1.0.0`.
 - Press `Create Deployment`, set fees, and press `Approve`.
 - Once you can see bids, select one and press `Accept Bid`.
 - Set fees, and press `Approve`.
 - Wait for PKT to enter your wallet ;)

## Deploying your own application

Assuming you have your application in Docker already, it is quite easy to transform it to be deployable on Akash. Following the [Stack Definition Language](https://docs.akash.network/sdl) in the documentation, you can see how you can configure each aspect.

If you need, you can take some inspiration from pre-existing applications. There are a few examples already in the Akashlytics Deploy Tool, that you can find by going to `Deployments` > `Create Deployment`. You can also take a look at how the [miner we used today](https://github.com/ovrclk/pkt-miner/blob/main/deploy.yaml) is configured. [Here](https://github.com/ovrclk/docs/blob/62714bb13cfde51ce6210dba626d7248847ba8c1/sdl/deployment.yaml) is yet another example.
 
Just don't forget to include a version, services, profiles, and deployment. The rest of the process should be self-explanatory after following this guide - assuming you do it vi
