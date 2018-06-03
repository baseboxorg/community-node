We will be building our primary cluster instance at the Linode data center in Atlanta Georgia, USA., where they offer an OC768 incoming network connection, with 40 Gbps in and 10 Gbps out. We believe that the incoming network connection will be critical for the Super Representative nodes.

Because the Tron Virtual Machine acts like a gigantic symmetric multiprocessor, we do not need one gigantic server instance, instead we will be building a cluster of server instances each with a specific task.


Our primary server cluster Instance will provide 196 Cores + 1 TB RAM + 20 TB SSD for the Tron Virtual Machine:  
1x GATEWAY NODE $960 each  
2x TRUSTED NODE $160 each  
5x WORKER NODE $960 each  
1x WITNESS NODE $240 each  
                                               
$10960 + .02¢ per GB data transfer. Estimated monthly expense $20,000

We will monitor the performance of this initial configuration and re-engineer accordingly.

Additional worker nodes will be deployed upon request by Tron Labs.


**`• Plans for hardware expansion`**  

We have discussed this project with John Arundel, noted author on the subject of Kubernetes and he has agreed to work with Community Node to develop a large scale deployment strategy. We will employ a variety of Cloud providers for geographic and resource diversity.




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

 

             
