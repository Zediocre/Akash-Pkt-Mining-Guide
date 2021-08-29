![Image2](https://user-images.githubusercontent.com/79159130/131248966-36ae0d51-6def-4693-8165-3d680b37cb30.png)



# Akash/Pkt Mining-Guide (in 5 Minutes)
(IMPORTANT) Please follow along with this easy explination 
first [here](https://www.youtube.com/watch?v=G-kFDTLMT0Y).
## 3 Easy Step Video Guide
 
 - [Setup Pkt](#Setup-Pkt)
 - [Akashlytics and Kepler](#Akashlytics-and-Kepler )
 - [Deploying On Akash](#Deploying-On-Akash)
## Setup PKT
 - Make a PKT wallet. use [this](http://pkt.world/wallet) one.
 - use Command Promt to Drag in folder and get private keys
 - Get a PKT address.
 
## Akashlytics and Kepler

 - Download and install [this](https://www.akashlytics.com/deploy) tool.
 - Open kepler wallet and Deposit Akash inside.
 - Send Over AKT ( 15 Recomended ).

## Deploying On Akash

 - Copy the contents from [this](https://github.com/ovrclk/pkt-miner/blob/main/deploy.yaml) file.
 - In the tool, go to `Deployments` > `Create Deployment`.
 - Continue forward by pressing Next > then use "Empty".
 - Paste the contents we copied.
 - Swap out the <PKT_WALLET> from `WALLET_ADDR=<PKT_Wallet>` to your wallet. (example in video below)
 - Press `Create Deployment`, set fees, and press `Approve`.
 - check your balance by pasting this code in command prompt: bin\pktctl --wallet getaddressbalances
 
