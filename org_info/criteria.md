Please send an application form containing the above information to the sr@tron.network



1. Have official website;

http://tron.communitynode.org/
 - also -
https://github.com/bondibox/community-node/



2. Provide company information:

Location 
  PO Box 39029
  Washington DC
  20016

Location of Server (start): 
  Linode Atlanta Data Center

Server type; 
  Cloud Based VM




3. Budget Expenditure and Technical Plan before June 26, 2018 (Reference fee: AWS $40,000)

(see below for detailed hardware configurations)  

  May 1 - May 28 alpha configuration $10 / month
  May 29 - June 21 beta configuration $40 / month
  June 22 - June 26 mock production configuration $320 / month





4. Hardware Expansion Plan after June 26, 2018
  June 27 - June 30 production level I $960 / month + $1000 per day data transfer
  July 1 - July 31 production level II $50,000 / month inclusive
  August 1 - December 31 production level III Estimate pending




 
5. Community Support Plan for 2018
We are active in the r/Tronix subgroup where we have become a go-to authority on the main net. 

We have entered into a strategic partnership with the Sesame Seeds SR Group to provide community support on a broader level than either of is able to provide by ourselves. Together we will be operating a Telegram help group to answer questions related to use of the Tron main net. We will also be pooling our collective knowledge and establishing best practices for the rest of the SR community.







6. List of key staff and their photos

CTO				[Jason Neely](./jason_neely.jpg)  
Devops			[xxxxx](./photos/xxxxx)  
Marketing	 	[Michael](./photos/michael)
Social Media
Outreach
Applications




7. Provide Background qualifications of key staff
• Chief Technical Officer / Founder
> Jason Neely has maintained a unix server almost constantly since 1998 when he installed RedHat and QTSS on his iMac. Soon after, he began work as an Apple Retail Representative, then went on to be a Tier 2 technician for Darwin Networks where he became Cisco certified. After the dot com bust he worked on the U.S. Congressional campaign of Andrew Horne, first as a volunteer who maintained the website and broadcasted emails, eventually writing copy and working directly with the communications team in a salaried position. From there, he formed Campaign Kickstart, a grassroots incubator, and developed an advocacy program for the Louisville Affordable Housing Trust Fund's Open the Door campaign. For the past 10 years he has been studying OOP and considers himself to be one of the last few Ruby on Rails enthusiasts.
 
• Devops Expansion Engineer
> John is a Docker & Kubernetes specialist located in Great Britain. (paste bio)

• Marketing Strategist
> Michael is the founder & chief strategist of xxxxxxx, a SEO, PPP & Remarketing specialty outfit. In his spare time he likes to run an Antminer that drives his family nuts.


• Social Media
> XXXXXXX is a prolific blogger who has 2,000 twitter followers.  


• Community Outreach  
> XXXXXXXX is a community organizer who has managed several grassroots campaigns.  

• Software Development  
>  XXXXXXXX has written several applications for iOS and Android and currently teaches Java at ___________.






8. Have nodes that can be tested by community members
  We have created a staging network, staging.communitynode.org which is a replica of the Tron main net and will allow the community to practice with wallets and to test the behavior of newly created dapps. It is already working in alpha with 1 witness and 2 seed nodes.



9. Community promotion efforts

• Social Media Following
  We have created accounts at Telegram and Twitter
  We are active on Reddit r/Tronix where they have 64,000 members.
  We openly publish our knowledge in a github repository to strengthen the SR community


• Livestream, 

• MEET UP






DETAILED HARDWARE CONFIGURATIONS


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
8 		GB RAM  
4 		CPU Cores  
96 		GB SSD Storage  
40 		Gbps Network In  
1 		Gbps Network Out  
2		GB Swap





# MOCK PRODUCTION CONFIGURATION
 2500 MHz Intel(R) Celeron(R) M processor
48 	GB RAM  
12 	CPU Cores  
768 	GB SSD Storage  
2	GB Swap
20 	TB Transfer (+ .02¢ per GB)
40 	Gbps Network In  
4 		Gbps Network Out  






# PRODUCTION LEVEL I

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








# PRODUCTION LEVEL II
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







# PRODUCTION LEVEL III
Kubernetes • Hadoop * Docker replicated network

TBD


