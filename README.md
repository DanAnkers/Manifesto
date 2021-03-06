# Manifesto

Network Engineers Manifesto 

**Key motivating factors:** 

- Data driven decisions.
- Excellence in all things. 
- Technical depth and no technology religion 
- Clarity of vision, clarity of execution 
- Lead the business in decisions related to transportation of packets
- Dedication to all our customers  
- "Good enough" is too low a bar


**Monitoring** 

- Monitor, at least:
- Per switch:
	- Interface pps,ups,mps,bitrate,drops,errors,buffer depth
	- CPU, Mem, ICMP messages generated 
	- STP states 
- Per router:
	- All routing protocol states 
	- Interface pps,ups,mps,bitrate,drops,errors,buffer depth
	- CPU, Mem, ICMP messages generated 
- Per Firewall:
	- Interface pps,ups,mps,bitrate,drops,errors,buffer depth
	- CPU, Mem, ICMP messages generated 
	- CPS, Throughput
	- Dropped connections 
	- ASIC drops 
- Per LB
	- Interface pps,ups,mps,bitrate,drops,errors,buffer depth
	- CPU, Mem, ICMP messages generated 
	- CPS, Throughput per VIP 
	- Dropped connections 
	- ASIC drops 
- Per AP
	- Interface pps,ups,mps,bitrate,drops,errors,buffer depth
	- CPU, Mem, ICMP messages generated 
	- Logged in users, failed login attempts
- Per Service
	- p99, p95 metrics for service latency:
		- For end to end transaction 
		- For TCP re-transmissions 
		- Latency to/drop server from all DCs
- All monitoring to be a single pane of glass for our users, API driven to allow them to extract their own 

		
**Deployment**

- Static routing to be avoided wherever possible
- Zero touch deployment for new gear
- Entirely templated configlets:
	- Base system configuration, including:  AAA, Logging,  
	- OSPF
	- STP 
	- BGP configlets 
	- IPSec tunneling 
- Absolutely no manual configuration pushes to production 
- Design and build a working lab for prototyping configuration 
- Goal to provide an API to our end users to deploy their infrastructure as they see fit  

**Remote offices**

- Regular random polling of remote users on office internet, general feeling of office network
- Managing this data over time to ensure we have total inclusion of our users 
- Dynamic monitoring and failover of IPSec tunnelling 
- Monthly SLA reporting of WAN performance based on 100% meshed pinging of remote offices 


**Reporting**

- Every single SNMP trap has to be actionable 
- Every single packet drop in our network has to be actionable
- Every single TCP re-transmission inside the borders of our administrative control has to be actionable
- Apply predictive algorithms to our graphing to alert of trends before they become issues.


**Personal Development**

- everyone must commit to self-improvement
- Certification track - optional but highly recommended 
- Regular hardware deep dives based on freely available vendor documentations, talks, presentations 

