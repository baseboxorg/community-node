*This document stays updated at https://github.com/bondibox/community-node/blob/master/sr_application/application.md*

> Please send an application form containing the above information to the sr@tron.network  




**`• Official Website`**  
[http://tron.communitynode.org/](http://tron.communitynode.org/)  
&  
[https://github.com/bondibox/community-node/](https://github.com/bondibox/community-node/)  




**`• Company information:`**  
The Community Node organization is an open source collaboration in the blockchain space. 

Our Mission is to become an intellectual asset for the community. The Tron project itself is open source, and we expect other cryptocurrencies to use the Tron application as a starting point for their blockchain networks. Other Distributed Proof of Stake cryptocurrencies may adopt Tron's Super Representative structure, and those Super Representatives will be creating organizations very similar to ours. We chose to make our project Open Source in order to provide a resource for those who come after us.

By sharing our IT strategies, it is our hope to strengthen the entire blockchain industry and advance the determination of best practices. 


**`• Company Location:`**  
c/o Jason Neely  
PO Box 39029  
Washington DC  
20016



**`• Social Media Following`**  
Our movement is still young and we are actively trying to bring in new members.  

Community Node on Telegram: [TRON Community Node & Super Representative](https://t.me/CommunityNode)  
Community Node on Twitter:  [@community_node](https://twitter.com/community_node)   
We are also active on Reddit [r/tronix]((http://reddit.com/r/tronix)).



**`• Community Support Plan for 2018`**  
We have created a staging network which is a replica of the Tron network and which will allow the community to practice with wallets and to beta test the behavior of newly created dapps. [It is already working in alpha](https://twitter.com/bondibox/status/991872321559261184) with 2 witnesses and 2 seed nodes.  We will continue the expansion of our test net to include solidity nodes and web wallets.

We will create a How To demonstration for a simple dapp game that flips a coin and pays tokens when guessed correctly. Users can upload this dapp to the staging network to experience the same functionality as the Tron main net.

We have entered into a strategic partnership with the Sesame Seeds SR Group to provide community support on a broader level than either of us is able to provide on our own. Together we are operating a [TRON Help Group](https://t.me/TronHelp) at Telegram to answer questions related to the Tron main net. 

We have contributed to the Tron Wiki and have pushed one set of changes.  

In keeping with our open source ideology, we will also be pooling our collective knowledge and establishing best practices for the rest of the SR community, and we will publish that information in a fork of the Official Tron documentation.





**`• Community promotion efforts`**   
We are holding a contest for the best main net java dapp, prize is 10,240 TRX payable from our node's first day of block rewards. Good for 10 dapp uploads on the Tron main net.



**`• Livestream`**  
https://www.periscope.tv/w/1ynKOAqXeEwJR  
Archived at YouTube:  
https://www.youtube.com/watch?v=PW0mWR9tVkw  







**`• List of key staff and their photos`**  
*CTO*				[Jason Neely](https://github.com/bondibox/community-node/blob/master/sr_application/jason_neely.jpg)    
*WAN Strategist*	Greg  
*dapp Education*		Colradi  
*UX Designer*		Duane Harrison



**`• Provide Background qualifications of key staff`**  
Chief Technical Officer / Founder  
> Jason Neely has maintained a *nix server almost constantly since 1998 when he installed RedHat and QTSS on his iMac. Soon after, he began work as an Apple Retail Representative, then went on to be a Tier 2 technician for Darwin Networks where he became Cisco certified. After the dot com bust he worked on the U.S. Congressional campaign of Andrew Horne, first as a volunteer who maintained the website and broadcasted emails, eventually writing copy and working directly with the communications team in a salaried position. From there, he formed Campaign Kickstart, a grassroots incubator, and developed an advocacy program for the Louisville Affordable Housing Trust Fund's Open the Door campaign (the legislature passed!). For the past 10 years he has been studying OOP and considers himself to be one of the last few Ruby on Rails enthusiasts.  


WAN Strategist  
> Greg is a SysAdmin for a leading Aerospace Manufacturer with over 90,000 users located around the globe. Over the past 12 years Greg has worked his way up the IT ladder learning many different products, software, and systems along the way. He currently holds a Bachelor in Networks and Communication and is near to completing his Technology focused MBA. Greg is an avid believer in the Tron Network Project and is excited to witness and be involved with its creation.

Application Education    
>  Colradi is a computer engineer in love with blockchain. He worked as an IT consultant and Java teacher for (too) many years in Madrid. Now he enjoys the inner peace of the mediterranean ocean, near Barcelona, and spends his days involved in a neverending Javascript project.

UX Designer
> Duane Harrison is a lead designer for one of the world’s largest airlines. Prior to this he has worked with a number of startups, overseeing and contributing to the design of mobile and web apps, one of which has featured in Apple’s WWDC keynote. Now based in Hong Kong, he is looking towards digital transformation in the financial space and sees huge potential in future applications that build on the Tron network.


**`• Testable nodes`**  
[Full sync was reached](https://github.com/bondibox/community-node/blob/master/sr_application/number_one.png) on April 27 with 300+ blocks produced.


**`• Location of Server:`**   
Linode Cloud Hosting  
Atlanta Data Center  


**`• Server type:`**  
Cloud Based VM  



**`• Budget Expenditure and Technical Plan before June 26, 2018`**  

$15          	. . .		Domain Registration CommunityNode.org  
$20          	. . .		 May 1 - May 28 alpha configuration  
$200         	. . .		 May 29 - June 26 beta configuration  
9,999 TRX  	. . .		 Super Representative Application Fee  
									------------------  
$235 + 9,999 TRX = Total expenses May 1 - June 26



We will be building our primary cluster instance at the Linode data center in Atlanta Georgia, USA., where they offer an OC768 incoming network connection, with 40 Gbps in and 10 Gbps out. We believe that the incoming network connection will be critical for the Super Representative nodes.

Because the Tron Virtual Machine acts like a gigantic symmetric multiprocessor cluster, we do not need one gigantic server instance, instead we will be building a cluster of server instances each with a specific task.


Each server cluster Instance will provide 196 Cores / 1 TB RAM for the Tron Virtual Machine:  
1x GATEWAY NODE $960 each | 16 Core / 300 GB   
2x TRUSTED NODE $160 each | 8 Core / 32 GB     
5x WORKER NODE $960 each  | 32 Core / 192 GB   
1x WITNESS NODE $240 each | 4 Core / 90 GB     
                                               
$10960 + .02¢ per Gb data transfer. Estimated monthly expense $20,000

We will monitor the performance of this initial configuration and re-engineer accordingly.


**`• Plans for hardware expansion`**  

We have discussed this project with John Arundel, noted author on the subject of Kubernetes and he has agreed to work with Community Node to develop a large scale deployment strategy. We will employ a variety of Cloud providers for geographical and resource diversity.



**`• Budget expenses after June 26`**  
$4,140  		. . .		June 27 - June 30 Production level I  
$ ? 			. . .		Bitfield Consulting  
$ ? 			. . .		Network Security Specialist  
$237,600	  	. . .		July 1 - December 31 Production level II  
10,240 TRX  	. . .		Promotional contest  
20,000 TRX		. . .		Colradi task bonus  
$30,000	. . .		Jason Neely salary from June 27 - December 31 (2.2%)  
? TRX				. . .		Other Contests and Promotions  

$271,720 + 20,000 TRX = Total Expenses from June 27 - December 31 2018 

Salaries are per annum maximums from June 27 - December 31 and will be based on the percentage of block participation.*  

Jason Neely < $30,000 (2.2% gross revenue) paid at the rate of 2 TRX per block until max payout is reached, and contingent upon the following expectations having been met:  
 ^ Able to meet technical requirements of Super Representative node  
 ^ Able to meet organization requirements of Super Representative node  
 ^ Continued operation of Super Representative node  
 ^ Hardware expansion goals met in timely manner

Colradi < 20,000 TRX paid upon completion of achievement levels:  
 ^ 10,000 TRX java based distributed application written  
 ^ 2,000 TRX dapp uploaded to test net  
 ^ 2,000 TRX token created for dapp  
 ^ 6,000 TRX dapp creation & upload HowTo document produced



| Name | GATEWAY NODE |
|---|---|
| Instance Type | Hi I/O |
| RAM | 	300 GB 
| CPU  | 	16 Cores
| SSD  | 	340 GB 
| Network  | 	40/10 Gbps 
| Cost | 	$960 month 
| Purpose | High bandwidth reverse proxy for workers & witness | 


| Name | WORKER NODE  |
|---|---|
| Instance Type |  CPU & Storage |
| RAM |          192 GB  | 	
| CPU  |         32 Cores  | 	
| SSD  |         3.8 TB  | 	
| Network |      40/10 Gbps  | 	$
| Cost |         960 month | 
| Purpose |      Provides flops and storage for TVM  | 


| Name |              WITNESS NODE  | 
|---|---|
| Instance Type   |   IPSec |  	
| RAM | 	          90 GB  | 
| CPU  | 	          4 Cores  | 	
| SSD  | 	          90 GB |  	
| Network  |          40/3 Gbps  | 	
| Cost | 	          $240 month | 
| Purpose |           IP Tunneled to the trusted nodes and proxy  | 


| Name |              TRUSTED NODE  | 
|---|---|
| Instance Type   |   IPSec |  	
| RAM | 	          32 GB | 
| CPU  | 	          8 Cores  | 	
| SSD  | 	      	640 GB|  	
| Network  |          40/2 Gbps  | 	
| Cost | 	          $160 month| 
| Purpose |           IP Tunneled to the witness node and proxy | 







*For the period of June 27 - December 31: Salaries, revenues, and some expenses are based on a maximum block production of 595,330