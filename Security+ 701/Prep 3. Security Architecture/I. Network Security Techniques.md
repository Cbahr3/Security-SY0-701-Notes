**Restricting Network Access** - security professionals must restrict access to networks
- *Perimeter Security* - keep unwanted remote users out of the network entirely through the use of firewalls and other controls
- *Network Access Control* - limit physical network access to authorized individuals and devices
To enforce security policies, we must be able to express them in technical terms
- *Rule Based* - restrict access based upon business logic
- *Role Based* - restrict access based upon the identity of an individual
- *Time Based* - restrict access based upon the time of day
- *Location Based* - restrict access based upon physical location

**Network Access Control**
- *Network Access Control* - intercepts network traffic coming from unknown devices and verifies that the system and user are authorized before allowing further communication, NAC uses 802.1x authentication
	- NAC Roles:
		- User and device authentication
		- *Role-based access* - authentication server provides additional user information, authenticator places user on a role-appropriate network based upon that information
		- *Posture checking* - verifying antivirus software presence, validating current signatures, ensuring proper firewall configuration, verifying presence of security patches, devices failing posture checks go into a quarantine VLAN
	- NAC Implementations:
		- Agent based
		- Agentless
		- In-band
		- Out of band

**Router Configuration Security** - routers perform basic filtering, they can reduce the load on firewalls
- *Router Access Control Lists* - restrict network traffic
	- *Standard Access Control Lists* - Perform filtering based upon source IP address
	- *Extended ACLs* - block traffic based upon more advanced criteria, such as source and destination IP addresses, source and destination ports, and the protocols used for a communication
	- Firewalls vs. Routers:
		- Firewalls are purpose specific and efficient
		- Firewalls have advanced rule capabilities
		- Firewalls offer advanced security functionality
Placing ACLs on routers reduces the burden on firewalls, quality of service (QoS) controls prioritize the critical network traffic

**Switch Configuration Security** - maintain the physical security of switches and other network gear, an attacker who gains physical access to your switch controls that portion of the network
- *VLAN Security* - disable automatic trunk negotiation to prevent VLAN hopping attacks
	- *VLAN Pruning* - limit the unnecessary exposure of VLANs by limiting the number of switches where they are trunked, especially for sensitive VLANs
	- *VLAN Trunk Negotiation* - deny the use of automatic VLAN trunk negotiation to limit the effectiveness of VLAN hopping attacks
	- *Port Security* - limit the devices that may connect to a network switchport by MAC address
		- *Static Port Security* - administrators manually configure valid MAC addresses for each port
		- *Dynamic Port Security* - switches memorize the first MAC address they see on each port and limit access to that address
	- *DHCP Snooping* - blocks malicious DHCP traffic

**Maintaining Network Availability** - maintaining network availability is a crucial security goal
- *Flooding Attacks* - overwhelm network devices
	- *SYN Floods* - fill connection state tables on firewalls with half-open connection entries
	- *MAC Floods* - fill switch's MAC address table with many entries, causing it to flood traffic on all ports
	- *Flood Guard Technology* - protects network devices against these attacks
	Port security is also effective against MAC flooding
	- *Routing Loops* - allow broadcast storms
		- *Spanning Tree Protocol (STP)* - prevents broadcast storms by implementing loop prevention
			- *BDPU Guard* - blocks malicious STP updates

**Network Monitoring** - firewall and network logs offer a rich source of security information
- Firewall Log Details:
	- Details about attempted connections
	- Timestamps
	- Relevant firewall rule
- Firewall Log Uses:
	- Security incident investigation
	- Network issue troubleshooting
	- Anomalous activity detection
	Full packet capture requires large storage capacity
	- *Network Flow Data* - captures connection details
		- NetFlow Records Capture:
			- Source and destination systems
			- Source and destination ports
			- Timestamps
			- Amount of data transferred
		NetFlow data is quite useful, it doesn't capture what was communicated but does identify who, when, and how much
- *Security Information and Event Management (SIEM)* - network security systems that automate the collection and analysis of logs from many different systems for security purposes
	- SIEM Log Sources:
		- Firewalls
		- Network devices
		- Servers
		- Applications
	SIEMs facilitate rapid analysis

**SNMP**
- *Simple Network Management Protocol (SNMP)* - automates routine network monitoring and management tasks, use SNMPv3, earlier versions have critical security flaws

**Isolating Sensitive Systems**
- *Network Segmentation* - separates systems of differing security levels, particularly sensitive servers may be placed in their own physically isolated security zone, physically isolated systems are called "air-gapped" systems
- *Jump Server* - allows administrators connections between zones, jump servers, jump boxes, and jump hosts are all the same thing, jump servers must be carefully secured

**Zero Trust Networking** - zero trust approaches to security place trust in individuals rather than networks, zero trust shifts the focus away from the perimeter protection and onto strong identity and access management
- *Identity and Access Management (IAM) Platforms* - are the foundation of zero trust approaches
Security information and event management (SIEM) and security orchestration, automation, and response (SOAR) platforms facilitate monitoring, cloud access security brokers (CASB) enforce security policies in the cloud
- *Endpoint Detection and Response (EDR) Platforms* - remediate endpoint security issues
- *Geofencing* - alerts when a device leaves a defined area

**Secure Access Service Edge (SASE)** - network security architectures are shifting away from a perimeter focus
- *Secure Access Service Edge (SASE)* - delivers a fully integrated network with ZTNA
	- SASE Components:
		- Software-defined networking (SDN)
		- Zero-trust network access (ZTNA)
		- Cloud access security brokers (CASBs)
		- Firewall as a service (FWaaS)
		- Other network security services
ZTNA is a medium-term objective, while SASE is a long-term goal, integrate ZTNA and SASE into your long-term design plans