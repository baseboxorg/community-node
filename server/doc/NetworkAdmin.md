With so little documentation during the development stages, there is a lot of confusion regarding the exact way that the Tron main net will operate. I have been running a Witness node for a few weeks and recently built a private test net, and I'm beginning to understand how it all works.

For the benefit of my fellow Super Representative candidates who are still mapping out a hardware migration, I'm sharing this. It goes with this project's Open Source ethos, and only goes to make the entire network stronger. 

First, some definitions. 

A *node* is a server that shares information on the p2p blockchain
A *witness node* is a server configured with a private key, which is available to produce blocks
A *super representative* is a witness node that has been elected to produce blocks
A *solidity node* is a node that runs a wallet server

There will be 100 witness node candidates. Those are witness nodes who have been voted upon by the community to run in the Super Representative election. Of them, 27 will be elected, every day, to be Super Representatives (SR's). There may be more than 100 witness nodes running, that's their prerogative in hopes they might get elected and move on to the SR election.

This establishes a level of trust for the candidates, and a higher level of trust for the elected SR's.

Every second, one witness node will produce one block. Then the next node will produce one block, and so on for 27 seconds until the cycle repeats itself. Whenever a SR produces a block, the other SR's validate the block, and then it gets shared on the blockchain, with all of the full nodes (seed nodes) who increase the availability of the information, possibly serving as links for passing the newly created blockchain among the Super Representatives. 

When each SR starts up, it will not be like it is in test net. Right now, all of the seed nodes are already running. In main net, each SR will add their seeds to the config file. When running the private testnet, I find it better if the seeds are running before starting up the primary witness node.  (the primary witness node is the first node to start up on day 1 of the blockchain. It creates a hash for the Zero block and then every node that starts up uses the same genesis criteria and checks their Zero block against the primary witness)

When main net is running I think a typical SR topography might look like this:

1 supercomputer configured as a witness node (alpha node)
Several failover servers configured exactly the same as the witness node. They will run in parallel and produce the same hash that the alpha node.
Lots of seed nodes designated by the witness node replicate the block produced to increase its availability
1 Config file is common among all of the witness nodes, to which each one adds their seed nodes.


https://github.com/bondibox/community-node/blob/master/server/doc/NetworkAdmin.md