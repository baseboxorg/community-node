> ** [To become a recommended Super Representative, candidates must meet the following requirements:*](https://medium.com/@Tronfoundation/tron-community-guidelines-ca10c2fcd444) **

> Please send an application form containing the above information to the sr@tron.network  



`Have official website;`

[http://tron.communitynode.org/](http://tron.communitynode.org/)  
&  
[https://github.com/bondibox/community-node/](https://github.com/bondibox/community-node/)  



`Provide company information:`

Location   
PO Box 39029  
Washington DC  
20016  

`Location of Server (start):`   
Linode Atlanta Data Center  

`Server type;`  
Cloud Based VM  


`Budget Expenditure and Technical Plan before June 26, 2018`

Although the recommended configuration is to use Amazon AWS with 25 Gbps network i/o, we are going to start with a service that offers a 40 Gbps in / 10 Gbps out network connection. The largest configuration available at this host is 16 core / 200 GB ram. We will test this against AWS to test the possibility that while the Tron main net is still young there may be more traffic headed into a Super Representative node than out. We will use whichever service performs better.




(see below for detailed hardware configurations)    

May 1 - May 28 alpha configuration $10  
May 29 - June 21 beta configuration $120
June 22 - June 26 Production Level I configuration $160


`Hardware Expansion Plan after June 26, 2018`

June 27 - June 30 production level II $4140  
July 1 - July 31 production level III $50,000 / month  
August 1 - December 31 production level IV Estimate pending  



`Community Support Plan for 2018`  
We are active in the r/Tronix subgroup where we have become a go-to authority on the main net.   

We have entered into a strategic partnership with the Sesame Seeds SR Group to provide community support on a broader level than either of us is able to provide on our own. Together we are operating a Telegram help group to answer questions related to use of the Tron main net. We will also be pooling our collective knowledge and establishing best practices for the rest of the SR community, and we will publish that information in a fork of the Official Tron documentation.

We have contributed to the Tron Wiki and have merged one change already.  




`List of key staff and their photos`

CTO				[Jason Neely](./jason_neely.jpg)    
WAN Strategist	[Greg](./photos/xxxxx)    
Marketing	 	
Social Media  
Outreach  
Applications   Colradi




`Provide Background qualifications of key staff`

• Chief Technical Officer / Founder  
> Jason Neely has maintained a *nix server almost constantly since 1998 when he installed RedHat and QTSS on his iMac. Soon after, he began work as an Apple Retail Representative, then went on to be a Tier 2 technician for Darwin Networks where he became Cisco certified. After the dot com bust he worked on the U.S. Congressional campaign of Andrew Horne, first as a volunteer who maintained the website and broadcasted emails, eventually writing copy and working directly with the communications team in a salaried position. From there, he formed Campaign Kickstart, a grassroots incubator, and developed an advocacy program for the Louisville Affordable Housing Trust Fund's Open the Door campaign (the legislature passed!). For the past 10 years he has been studying OOP and considers himself to be one of the last few Ruby on Rails enthusiasts.  


• WAN Strategist  
> Greg is a SysAdmin for a Fortune 500 company. He is responsible for a network of 


• Application Education    
>  Colradi is a computer engineer in love with blockchain. He worked as an IT consultant and Java teacher (the same language in which Tron blockchain has been coded) for (too) many years in Madrid. Now he enjoys the inner peace of the mediterranean ocean, near Barcelona, and spends his days involved in a neverending Javascript project.






`Have nodes that can be tested by community members`  
  
We have created a staging network which is a replica of the Tron network and which will allow the community to practice with wallets and to beta test the behavior of newly created dapps. It is already working in alpha with 1 witness and 2 seed nodes.  We will continue the expansion of our test net to include solidity nodes and web wallets.




`Community promotion efforts`

• Social Media Following  
We have created accounts at Telegram and Twitter  
We are active on Reddit r/Tronix where they have 64,000 members.  
We openly publish our knowledge in a github repository to strengthen the SR community  
We are holding a contest for the best main net java dapp, prize is 10,240 TRX* good for 10 dapp uploads

• Livestream,   
https://www.periscope.tv/w/1ynKOAqXeEwJR
Archived at YouTube:
https://www.youtube.com/watch?v=PW0mWR9tVkw


• MEET UP  






`DETAILED HARDWARE CONFIGURATIONS`  


# ALPHA TEST CONFIGURATION  
Debian GNU/Linux 9.1 (stretch) 4.15.12-x86_64  
2500 MHz Intel(R) Celeron(R) M processor  
4	 	GB RAM    
2 		CPU Cores    
46 		GB SSD Storage    
40 		Gbps Network In    
1 		Gbps Network Out    
2256	SWAP  



# BETA TEST CONFIGURATION  
2500 MHz Intel(R) Celeron(R) M processor  
24	 	GB RAM  
8	 	CPU Cores  
384 	GB SSD Storage  
16		TB Transfer (+ .02¢ per GB)
40 		Gbps Network In  
2	 	Gbps Network Out  



# PRODUCTION LEVEL I CONFIGURATION  
2500 MHz Intel(R) Celeron(R) M processor  
200 	GB RAM    
16 		CPU Cores    
340 	GB SSD Storage    
2		GB Swap  
9 		TB Transfer  (+ .02¢ per GB)  
40 		Gbps Network In    
10 		Gbps Network Out    






# PRODUCTION LEVEL II  

-- PRIMARY INSTANCE --  
2500 MHz Intel(R) Celeron(R) M processor  
200 	GB RAM    
16 		CPU Cores    
340 	GB SSD Storage    
2		GB Swap  
9 		TB Transfer  (+ .02¢ per GB)  
40 		Gbps Network In    
10 		Gbps Network Out    


-- FAILOVER INSTANCE --  
2500 MHz Intel(R) Celeron(R) M processor  
200 	GB RAM    
16 		CPU Cores    
340 	GB SSD Storage    
2		GB Swap  
9 		TB Transfer  (+ .02¢ per GB)  
40 		Gbps Network In    
10 		Gbps Network Out    








# PRODUCTION LEVEL III
-- PRIMARY INSTANCE --  
AWS 	x1.16xlarge  
64 		cores  
1 		TB RAM  
1		TB SSD(EBS)  
25		Gbps Network  

-- FAILOVER INSTANCE --  
2500 MHz Intel(R) Celeron(R) M processor  
200 	GB RAM    
16 		CPU Cores    
340 	GB SSD Storage    
9 		TB Transfer  (+ .02¢ per GB)  
40 		Gbps Network In    
10 		Gbps Network Out    







# PRODUCTION LEVEL IV
Kubernetes • Hadoop * Docker replicated network  

TBD  




\* 10,240 Prize will be drawn from this node's first day of block rewards




