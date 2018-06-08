We will be building our primary cluster instance at the Linode data center in Atlanta Georgia, USA., where they offer an OC768 incoming network connection, with 40 Gbps in and 10 Gbps out. We believe that the incoming network connection will be critical for the Super Representative nodes.

Because the Tron Virtual Machine acts like one big symmetric multiprocessor cluster, we do not need a one-size-fits-all server instance, instead we will be building several server instances each with a specific task.

A Super Representative faces two technical responsibilities. The mission critical component is running a well protected Witness Node. Then you must make available lots of flops and storage for TVM.

Our Primary cluster surrounds our Witness node with 6 Sentry nodes, which connect to the Witness via an IPSec tunnel. This cloaks the witness from the outside world, and allows it to advertise a private IP address. The 6 Sentry nodes act as the point of contact for the witness node, meaning a successful DDoS attack would have to discover and compromise all 6 Sentries. The Sentries will then be surrounded by unprotected Full Nodes which do the heavy lifting of the network. 8 of these nodes are configured to provide the most resources per dollar, and 4 are provisioned with 40/10 Gbps network connections. This ought to provide an optimal combination of storage, CPU and burst availability.

Our primary deployment cluster will provide **280 Cores + 1620 GB RAM + 23 TB SSD** for the Tron Virtual Machine:  

1x Witness Node $160 each  
6x Sentry Nodes $160 each  
2x High Mem High I/O Node $960 each  
2x High CPU High I/O Node $960 each  
8x Worker Nodes $320 each

$7520 + .02¢ per GB data transfer after the first 330 TB.  

We will monitor the performance of this initial configuration and re-engineer accordingly.



8x Worker Nodes + 4x High I/O Nodes
 |
6x Sentry Nodes
 |
Witness Node


**`• Plans for hardware expansion`**  

We have discussed this project with John Arundel, noted author on the subject of Kubernetes and he has agreed to work with Community Node to develop a large scale deployment strategy. We will employ a variety of Cloud providers for geographical and resource diversity.

**`• Budget Expenditure and Technical Plan after June 26`**  
Percentages are of daily block rewards earned.  
80% - Voter Rewards Program  
7% - Resource Deployments
13% - Operating Expenses

Since we will be spending 7% of revenue on node deployments, our deployment will scale with the value of TRX. For every .04¢ gain in TRX price we will add another cluster.

We will distribute up to 80% of daily block rewards back to the voters who elect us to office, through a program that draws payouts from a slowly accruing payout account which maxxes out at 4 Million TRX. When the Super Representative Program ends in 2021, we will use all of the expertise we've gained to continue to run the Tron network. We will spend the entire 4 Million TRX that we've accrued in the payout account to buy hardware infrastructure on an enterprise level.





| Name | I/O High MEM |
|---|---|
| RAM | 	300 GB 
| CPU  | 	16 Cores
| SSD  | 	340 GB 
| Network  | 	40/10 Gbps 
| Transfer | 9 TB |
| Cost | 	$960 month 
| Purpose | High Memory / High bandwidth node | 


| Name | I/O High CPU |
|---|---|
| RAM |          192 GB  | 	
| CPU  |         32 Cores  | 	
| SSD  |         3.8 TB  | 	
| Network |      40/10 Gbps  | 	
| Transfer |  20 TB |
| Cost |         960 month |
| Purpose | High CPU / High bandwidth node |  


| Name |  SENTRY NODE & WITNESS NODE  | 
|---|---|
| RAM | 	          32 GB | 
| CPU  | 	          8 Cores  | 	
| SSD  | 	      	640 GB|  	
| Network  |          40/2 Gbps  | 	
| Transfer | 16 TB |
| Cost |      $160 month| 
| Purpose |   IPSec Tunneled Witness & Witness Border Nodes  | 
         

             
| Name | WORKER NODE  |
|---|---|
| RAM | 	64 GB 
| CPU  | 	16 Cores
| SSD  | 	1280 GB 
| Network  | 	40/4 Gbps 
| Transfer | 20 TB |
| Cost | 	$320 month 
| Purpose |  Lowest Resource Cost | 


