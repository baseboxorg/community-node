
[https://mp.weixin.qq.com/s/1E1EJWml6AIwpk0vqotK7A](https://mp.weixin.qq.com/s/1E1EJWml6AIwpk0vqotK7A)  (translated)

> The super representative is the core manager of the TRON community in the pool field. They will perform basic duties such as block production and paying the expenses of the TRON network. They obtain corresponding revenue.

> Every 24 hours, the super delegates and super representative candidates will accept the supervision and choice of the voters.

> Every coin holder has the opportunity to become a super representative of the TRON community in the pool field, but in order to make the pool field, TRON network, and community run smoothly, efficiently and well, we will formulate a series of standards, and rules for meeting these standards.

> We will give certain publicity recommendations to increase our recommended super representatives' chances of being elected super delegates.


#FAQ#


***What is the Tron Main Net?***

The Tron main net, which launches on May 31, 2018, is a peer-to-peer (p2p) network that hosts the Tron blockchain.

***What is the Tron blockchain?***

The Tron blockchain will be a network for transferring the Tron cryptocurrency, known as TRX. It will also allow contract creation, and application deployment.

***How will the blockchain work?***

The blockchain will consist of 27 privately run computer nodes. They will create and verify the new blocks that are added to the chain. TRX wallets will connect to the blockchain to retrieve balance information and allow the transfer of TRX between addresses. There will be a contract creation feature similar to Ethereum. It will also host distributed applications, or *dapps*.

***What is the Community Node project?***

The Community Node project is a proposal to manage and operate a node on the Tron main net. It is an Open Source proposal, which means if and when the proposal is adopted and the organization is formed, it will be owned 100% by the public, managed by the owners through an election process. In the meantime, we are committed to sharing all of our accrued knowledge by printing it in our public repository.

***What's the difference between a node and a witness node and a Super Representative node?***

Definitions:  
 • A *node* is a server that shares information on the p2p blockchain  
 • A *witness node* is a node that is configured with a private key and is available to produce blocks.  
 • A *super representative*  (aka Super Delegate) is a witness node that has been elected to produce blocks  
 • Full Node runs without a private key  
 • Solidity node is a wallet server  
 - Super Representative produces blocks  
 - Other SRs validate the block  
 - Full nodes are specified in the witness node's config file so only trusted nodes are used.  
 - Full nodes keep a copy of the blockchain and also pass new transactions to the witness producing the block.  
 - Solidity nodes only keep a copy of the blockchain, and not the pending transactions. All info available to the wallet is validated.  

***How much does the Super Representative earn?***

Tron labs will pay each Super Representative 32 TRX per block. Only the 27 super representative nodes get to produce blocks. They take turns making one block per second, so about 2.2 blocks a minute for each of the Super Representatives. The winners hold their positions for 24 hours, and every day there is another election. Some SR's will win the election 365 days a year. Others may end up winning a fraction of the time, if at all. Even if the candidate node loses the SR election, they must maintain a presence and the associated expenses. The most a SR can earn during the year is about 34 Million TRX.

***How much does it cost to be a Super Representative?***

There's a lot of expense. Tron recommends a technical budget of about $40,000 *a month*. OCN is currently building a cluster of 150 AMD EPYC 24 core CPUs.


***Can anyone run a node?***

Yes. Everyone is welcome to run a witness node and try to become a "Super Representative" node. In order to be recommended for the Super Representative post, you must meet a set of rigorous criteria. In order to become a Super Representative you must win a daily election.


***Let me follow the money.***

Super Representative witness nodes may choose to share their rewards with the TRX community, as is sometimes seen with other DPoS cryptocurrencies. 

Some Super Representatives are partners with Tron and have the backing of billions of TRX. Someone like OCN who has spent such an enormous sum on infrastructure doesn't stand a chance of losing the election. Tron has 15 such partners. It's unlikely that they will directly reward the TRX voters who elected them. For one, they own most of the TRX that voted them into position. Secondly, they can win the election without the help of the average TRX voter. 

Some of the Super Representatives will spend all of their earned TRX rewards on their technical operating budget. This is in their own self interest as it creates the framework over which their applications will run. Even though a TRX voter won't get direct compensation from Super Representatives like OCN, a TRX voter may still wish to vote for them to ensure the stability of the Tron network. In this regard, the TRX voters expect some benefit from their votes, be it capital investment in the Tron network or direct compensation.


***Someone said something about earning TRX. How does that work***

Community Node hopes to reward the voters who elect it to Super Representative 




***What's a dapp?***

A dapp is like the apps on your phone. In the beginning of the internet, web pages didn't change. Nowadays most web pages load *dynamic* content that they pull from a database. They have account logins, let you post articles and comments, etc.  Even though my weather app can show me updated and detailed information for every place around the globe, the app is pretty small.

Developers who have written dapps for the Tron network can upload them when they're ready for a fee of 1024 TRX. This "burns" the coins and removes them from circulation. This is the only "coin burn" there is planned for the Tron main net.

***What's a "staging network"?***

The Community Node staging network is a carbon copy of the real Tron network. It runs on our private servers and we provide it to the community as a free service. With it you can practice using a wallet. You can click a button and we'll put 1,000,000 free xTRX tokens in your account, and you can practice sending and receiving with them, as well as practice creating cold wallets and other security measures.

When your dapp is ready, you can spend 1024 of your free xTRX tokens and upload your dapp to the staging network just as you would with the real Tron main net. Uploading a Tron dapp to the real Tron main net will cost 1024 TRX so it's not something you want to mess up.


***Do I have to have a dapp thingy?***

Building dapps is not a requirement of Community Node members, though we would love to include developers on our team. We are doing everything we can to support the dapp development community. Dapp developers don't have to be core members of the team.





***How do dapps work?***

A dapp is like a bridge. On one side is what you see on your phone. On the other side is an API, or *application procedure interface*. That means if you tell it one thing, it will respond with a particular behavior. The commands that the dapp sends to the API are called RPC, *remote procedure calls.*  To view this webpage, your web browser issued a "GET" RPC to the webserver's API. 

***Why do dapps need a blockchain?***

They don't need a blockchain, but it gives the developer a decentralized way of running the dapp. Instead of relying on a single server, the dapp is hosted by hundreds of nodes on the blockchain. It removes all server management and you get a 'set it and forget it' convenience.

***What's another advantage?***

Dapps uploaded to the blockchain are permanent and incorruptible. They can not be censored.

***Walk us through the dapp process.***

We are sure the Tron network will support Java applications. I would also expect to see Python included, as well as Ruby and other high level languages. A developer will write their program in the language of their choice. Above I said that the information was permanent, but there's a gotcha. A developer has two choices. The first choice is to include media and content in the app itself, at which point it becomes a part of the blockchain. The second choice is to set the app to load information dynamically, like my weather app does. The dapp for my weather app is just an empty shell that looks pretty, then when the dapp runs it loads dynamic content via API RPC. Since most websites display dynamic content and use a database to store information, it means that your cat videos won't actually become a permanent part of the blockchain.

***I'm a web developer. That sounds like a security risk to have your database connection info included in the blockchain.***

Your dapp will get turned into runtime bytecode before it's uploaded.

