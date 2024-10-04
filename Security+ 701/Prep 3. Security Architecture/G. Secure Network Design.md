**Security Zones** - firewalls segment networks into security zones to protect systems of differing security levels
- *Zero Trust* - system gains no trust based solely on network location
- *Extranet* - intranet segment extended to business partners
- *Honeynet* - decoy network designed to attract attackers
- *Ad Hoc Network* - temporary network that may bypass security controls
Firewalls reduce the attack surface
- *East-West Traffic* - network traffic between systems located in the data center
- *North-South Traffic* - network traffic between systems in the data center and systems on the internet

**VLANs and Network Segmentation**
- *VLANs* - virtual LANs (VLANs) separate systems on a network into logical groups based upon function, regardless of physical location, VLANs extend the broadcast domain
	- Configuring VLANs:
		- Enable VLAN trunking
		- Assign switchports to VLANs

**Security Device Placement** - security devices must be properly placed within a network
- Network Traffic Collectors:
	- Intrusion detection and prevention sensors
	- Network taps
	- Port mirrors
Aggregation (or distribution) switches connect downstream access switches to each other, SPAN ports receive a copy of all traffic seen on a switch
- *Port Mirroring* - allows the monitoring of traffic on a single switchport
- Security Information and Event Management:
	- Gather information using collectors
	- Analyze information with a centralized aggregation and correlation engine
	- Place collectors near the systems generating records
	- Place the correlation engine in a secure location
Proxy servers and content filters typically belong in the DMZ
- VPN Concentrators:
	- Aggregate remote user connections
	- Often reside in their own VLAN, where access controls may restrict remote user activity
	- Sophisticated designs may use multiple VLANs for different user roles
- *SSL Accelerators* - handle the difficult cryptographic work of setting up TLS connections
- *Load Balancers* - distribute connection requests among multiple servers
SSL accelerators and load balancers belong in the DMZ
- *DDoS Mitigation Tools* - belong as close to the internet as possible
Purchasing DDoS mitigation services from your ISP is an ideal approach

**Software-defined Networking (SDN)** - software-defined networking treats network functionality and implementation details separately, reconfiguring traditional networks requires reconfiguring devices
- *Control Plane* - responsible for making routing and switching decisions
- *Data Plane* - responsible for carrying out the instructions of the control plane
Software-defined networking (SDN) separates the control plane from the data plane, SDN makes the network programmable
- SDN Security Benefits:
	- Allows granular network configuration
	- Facilitates faster response to security incidents
SDN increases network complexity, SD-WAN extends the benefits of SDN to wide-area networks connecting remote sites